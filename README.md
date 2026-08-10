# Olá! Eu sou Jaasiel Silva 👋

Desenvolvedor Full Stack apaixonado por construir produtos SaaS do zero — do modelo de dados ao deploy em produção.

🌍 **Localização:** Nasci em Belém/PA e moro em São Paulo, Brasil 🇧🇷

💼 **Atualmente:** Analista de Sistemas Jr no **Grupo GPS**, atuando como desenvolvedor full stack e construindo soluções SaaS.

🚀 **O que eu construo:**
Nos últimos meses venho desenvolvendo e operando diversas plataformas SaaS multi-tenant em produção, cobrindo áreas como gestão jurídica, gestão empresarial, atendimento (helpdesk), agendamento para profissionais de saúde e serviços automotivos — sempre com autenticação JWT/RBAC, multi-tenancy real e integração com WhatsApp (Z-API/WAHA).

---

### 🌟 Projeto em destaque: Zelly

SaaS de contratos recorrentes e ordem de serviço para prestadores de manutenção técnica (climatização, dedetização, facilities, elevadores) — produto próprio, construído do zero: modelagem de domínio, multi-tenancy real, cobrança recorrente e deploy em produção.

![Java](https://img.shields.io/badge/Java%2021-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot%203-6DB33F?style=flat-square&logo=spring&logoColor=white)
![Angular](https://img.shields.io/badge/Angular%2022-DD0031?style=flat-square&logo=angular&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL%208-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Asaas](https://img.shields.io/badge/Pagamentos-Asaas-00C2A8?style=flat-square)
![JWT](https://img.shields.io/badge/Auth-JWT%20%2B%20RBAC-000000?style=flat-square&logo=jsonwebtokens&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

- **Multi-tenant real:** isolamento por `empresa_id` via `@TenantId` (Hibernate), provado por teste de isolamento
- **Cobrança recorrente via Asaas:** integração com gateway de pagamento (sandbox), webhook de confirmação e régua própria de dunning para inadimplência
- **Auth completa:** login, refresh token rotacionado, RBAC, convite de usuário, recuperação de senha
- **Núcleo do produto:** `Contrato` (vigência, reajuste por índice, renovação), agenda com visitas automáticas, ordem de serviço (checklist, foto, assinatura)
- **Ciclo comercial do SaaS:** planos, quotas, painel do dono, impersonação auditada, relatórios com MRR

🔗 [zelly.digital](https://zelly.digital)

---

### 💼 LexCRM — vendido para clientes reais

Plataforma de gestão jurídica integrada, em produção atendendo escritórios/clientes reais — não é projeto de portfólio, é sistema pago em uso.

![Java](https://img.shields.io/badge/Java%2017-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=spring&logoColor=white)
![Thymeleaf](https://img.shields.io/badge/Thymeleaf-005F0F?style=flat-square&logo=thymeleaf&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring%20Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

- **Controle de processos e prazos:** cadastro de processos, controle de prescrição (prazo prescricional) e radar de vencimentos — evita perda de prazo, o maior risco de um escritório
- **Financeiro e agenda** integrados ao processo/cliente, com geração de laudos
- **RBAC granular:** políticas de acesso e permissões por usuário/perfil, painel de segurança dedicado
- **Multi-cliente:** painel SuperAdmin com gestão de contas, chamados de suporte e monitoramento de backup automatizado
- Deploy em produção via Docker (ambientes de produção e homologação separados)

---

### 🚗 LavaRapido — vendido para clientes reais

Sistema de gestão para lava-jato multi-empresa, também em produção com cliente pagante — do agendamento à cobrança.

![Java](https://img.shields.io/badge/Java%2017-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=spring&logoColor=white)
![Thymeleaf](https://img.shields.io/badge/Thymeleaf-005F0F?style=flat-square&logo=thymeleaf&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![WhatsApp API](https://img.shields.io/badge/WhatsApp%20API-25D366?style=flat-square&logo=whatsapp&logoColor=white)

- **Multi-empresa:** cada cliente do SaaS opera isolado, com painel MASTER para visão global
- **Operação completa:** clientes, veículos, agendamento, mensalistas (planos recorrentes), catálogo e vendas
- **Retenção automatizada:** detecção de cliente sem retorno, campanha de aniversário e pesquisa de satisfação, tudo disparado via WhatsApp (integração Meta Cloud API + Z-API)
- **Painel de fila em tempo real** para acompanhamento operacional do lava-jato
- **Observabilidade:** stack própria de monitoramento (Prometheus, Grafana, Loki, Alertmanager) e backup monitorado
- Deploy em produção e homologação, com pipeline de deploy via Docker Compose

---

- ### Frontend:
<a href="https://www.w3.org/TR/html52/" target="_blank">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" />
</a>
<a href="https://www.w3.org/Style/CSS/" target="_blank">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />
</a>
<a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
</a>
<a href="https://www.typescriptlang.org/" target="_blank">
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
</a>
<a href="https://angular.io/" target="_blank">
  <img src="https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white" alt="Angular" />
</a>
<a href="https://reactjs.org/" target="_blank">
  <img src="https://img.shields.io/badge/React.js-61DAFB?style=for-the-badge&logo=react&logoColor=white" alt="React.js" />
</a>

- ### Backend:
<a href="https://spring.io/projects/spring-boot" target="_blank">
  <img src="https://img.shields.io/badge/Java_with_Spring_Boot-6DB33F?style=for-the-badge&logo=spring&logoColor=white" alt="Java with Spring Boot" />
</a>
<a href="https://expressjs.com/" target="_blank">
  <img src="https://img.shields.io/badge/Node.js_with_Express-339933?style=for-the-badge&logo=node.js&logoColor=white" alt="Node.js with Express" />
</a>

- ### DevOps / Infra:
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white)

#### Databases:
![SQL Server](https://img.shields.io/badge/SQL%20Server-CC2927?style=for-the-badge&logo=microsoftsqlserver&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)

#### Workstation Tools:
![VScode](https://img.shields.io/badge/vscode-4285F4?style=for-the-badge&logo=vscode&logoColor=white)&nbsp;
![Claude Code](https://img.shields.io/badge/Claude%20Code-D97757?style=for-the-badge&logo=anthropic&logoColor=white)&nbsp;
![Cursor](https://img.shields.io/badge/Cursor-000000?style=for-the-badge&logo=cursor&logoColor=white)&nbsp;

🌱 **Aprofundando agora em:**
- Arquitetura multi-tenant e observabilidade (Prometheus/Grafana/Loki) em ambientes Docker com múltiplos serviços
- Angular 17+ no frontend de aplicações SaaS

📫 **Vamos nos conectar!**
Se você está interessado em colaborar em projetos ou só quer bater um papo sobre tecnologia, fico à disposição.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-JaasielSilva-blue)](https://www.linkedin.com/in/jaasiel-silva-b86b75303/)

<div>
<a href="mailto:jasiel1@outlook.com">
  <img src="https://img.shields.io/badge/-Gmail-%23333?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail" target="_blank">
</a>
</div>&nbsp;&nbsp;

<img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=8F0D87&height=120&section=footer"/>
