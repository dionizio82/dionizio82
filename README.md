# Heber Dionizio

**Desenvolvedor full stack com IA e contador (CRC-PR 054.502/O-4) · Curitiba, PR**

Escrevo e opero sistemas para a rotina fiscal, contábil e jurídica brasileira. Backend em Python, frontend em TypeScript, infraestrutura própria. Sou o criador do [NotaNoZap](https://www.notanozap.com.br) e o contador responsável da Leão Digital Contabilidade.

> A maior parte do meu código fica em repositórios privados, porque roda em produção com dados fiscais de clientes. Esta página descreve o que cada sistema faz e como foi construído. Posso apresentar código e arquitetura em conversa.

## Em produção

| Sistema | O que faz | Stack |
|---|---|---|
| **[NotaNoZap](https://www.notanozap.com.br)** | SaaS de NFS-e para prestadores e escritórios contábeis. Emite em dois protocolos (ABRASF 2.04 por SOAP e Emissor Nacional por REST com mTLS), pelo portal ou por mensagem no WhatsApp, em texto ou áudio. | Python 3.12, Django 5.2, DRF, PostgreSQL 16, React 18, Docker |
| **[Balança PJe](https://www.heberdionizio.com.br/balanca-pje)** | Liquidação de sentenças trabalhistas. Extrai a decisão com LLM, com citação de página por item, e opera o PJe-Calc oficial por automação. O caso de referência fecha ao centavo. | FastAPI, Pydantic, Playwright, Next.js 16 |
| **[Dados Abertos RFB](https://rfb.leaodigital.tech)** | ETL mensal da base completa de CNPJs da Receita Federal, com consulta web, API e histórico de alterações. Promoção para produção por troca de schema, com cerca de 2 s de indisponibilidade. | Python, PostgreSQL, FastAPI, Next.js |
| **Carteira Limpa** | Contadores renunciam em lote a vínculos no REDESIM pela API Serpro Integra Contador, com comprovante oficial de cada renúncia. | FastAPI, HTMX, PostgreSQL, Redis, ARQ |
| **Cofre de Certificados** | Serviço central de certificados A1 ICP-Brasil: cifra por envelope AES-256-GCM, rotação de chave, assinatura XMLDSig por API e auditoria de cada leitura. | FastAPI, PostgreSQL, Alembic |
| **Empreenda Contábil** | Marketplace gratuito que conecta escritórios de contabilidade e profissionais contábeis. | Next.js 16, Drizzle, PostgreSQL |

Em homologação: **DJE Empresas**, monitoramento do Domicílio Judicial Eletrônico (CNJ/PDPJ) com ciência automática por regra de prazo.

## Como eu trabalho

- **De ponta a ponta, sozinho.** Modelo de dados, API, interface, deploy, backup, cobrança e suporte ao cliente.
- **IA onde ela resolve.** Extração estruturada de documentos com citações, transcrição de áudio com Whisper e um servidor MCP próprio que dá a agentes acesso aos sistemas com escopo por chave e trilha de auditoria. Claude Code faz parte do meu fluxo de desenvolvimento.
- **Infraestrutura própria.** 77 containers em 14 stacks Docker Compose, Traefik, Cloudflare Tunnel, acesso administrativo só por Tailscale, SSO, backup cifrado com teste de restauração automatizado e monitoramento.
- **Regra de negócio na origem.** Sou contador desde 2007. Fui CFO, fundador de escritório de contabilidade e gerente no Banco do Brasil antes de programar.

## Stack

**Backend:** Python, Django, Django REST Framework, FastAPI, Pydantic, SQLAlchemy, Celery, ARQ · Node.js
**Frontend:** TypeScript, React, Next.js, Vite, Tailwind CSS, shadcn/ui, HTMX
**Dados e infraestrutura:** PostgreSQL, Redis, MinIO, Docker, Linux, Traefik, Nginx, Cloudflare
**Integrações:** NFS-e, certificado digital A1, mTLS, XMLDSig, Serpro Integra Contador, PDPJ, Asaas, Banco Inter, Cora, WhatsApp

## Formação

- Tecnólogo em Análise e Desenvolvimento de Sistemas, Faculdade AIEC (2021)
- MBA Executivo em Marketing e Mídias Digitais, FGV (2023)
- MBA em Auditoria Integral, UFPR (2007)
- Bacharel em Ciências Contábeis, UFPR (2005)

## Contato

Disponível para atuar como desenvolvedor full stack e para projetos de diagnóstico, integração e sistemas sob medida.

[heberdionizio.com.br](https://www.heberdionizio.com.br) · [LinkedIn](https://www.linkedin.com/in/heberdionizio) · contato@heberdionizio.com.br · [WhatsApp](https://wa.me/5541992555891)
