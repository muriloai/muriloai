# Murilo de Abreu Inácio
### Analista de Sistemas e Desenvolvedor Full Stack (.NET e Angular)

Atuo com **desenvolvimento de software há 6 anos** e tenho mais de 13 anos de experiência em TI. Minha experiência abrange levantamento de requisitos, modelagem de dados, implementação de regras de negócio, desenvolvimento de interfaces e suporte em produção.

Minha stack principal é **C#, .NET (Framework e Core), Angular (v7 ao v14), TypeScript, JavaScript e SQL Server**, com bastante prática em refatoração e modernização de código legado.

---

### Experiência em produção e resultados práticos

<table>
  <tr>
    <td width="33%" valign="top">
      <strong>Modernização de ERP de saúde (900+ telas)</strong>
      <p>Participei da migração do frontend do Angular 7 para o 14, escrevi mais de 130 testes automatizados com Jasmine, Karma e Cypress para proteger regras críticas de negócio e atualizei mais de 100 dependências em .NET Framework. Essa vivência com sustentação e evolução de código deu origem aos laboratórios de modernização (<a href="https://github.com/muriloai/dotnet-modernization-lab">.NET</a> e <a href="https://github.com/muriloai/angular-modernization-lab">Angular</a>) e às demonstrações de integração listadas abaixo.</p>
    </td>
    <td width="33%" valign="top">
      <strong>Automação de coleta em campo (17,5 min → 1,5 min)</strong>
      <p>Desenvolvi o <a href="https://github.com/muriloai/winforms-survey-data-entry">Survey Data Entry</a>, um sistema desktop em C# que reduziu o tempo de digitação de fichas presenciais de 17,5 minutos para 1,5 minuto por cadastro. Concebido em 2014 sobre MySQL, o projeto foi refatorado para operar com SQLite embutido (zero configuração), transações ACID e interface limpa, com toda a <a href="https://github.com/muriloai/winforms-survey-data-entry/blob/main/HISTORIA.md">evolução documentada</a>.</p>
    </td>
    <td width="33%" valign="top">
      <strong>Migração de legados e relatórios financeiros</strong>
      <p>Conduzi a transição de sistemas internos escritos em ASP clássico e ASPX para versões modernas em PHP com MySQL, além de modelar consultas, visões analíticas e relatórios corporativos de faturamento e contas a receber, experiência demonstrada em projetos como <a href="https://github.com/muriloai/cobranca-web-dotnet">Cobrança Web</a> e <a href="https://github.com/muriloai/crystal-reports-service-billing">Service Billing</a>.</p>
    </td>
  </tr>
</table>

---

### Projetos públicos em destaque

Aplicações completas, ferramentas desktop e laboratórios técnicos com decisões de arquitetura, instruções de execução e cenários reais de negócio documentados.

#### Sistemas Web, APIs e Arquitetura Corporativa

<table>
  <tr>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/muriloai/cobranca-web-dotnet">Cobrança Web</a></h4>
      <p>Sistema de negociação e acompanhamento de dívidas que integra uma operação legada em ASP.NET MVC 5 (via ADO.NET) a uma API em .NET 8 sobre o mesmo banco SQL Server. Resolve o desafio de evoluir contratos HTTP sem quebrar consumidores existentes: mantém a leitura consolidada na rota <code>v1</code> enquanto expõe na <code>v2</code> o detalhamento de parcelas e vencimentos com preservação do centavo residual e transição de estado por <em>stored procedures</em>.</p>
      <p><strong>Stack:</strong> <code>C#</code> <code>.NET Framework 4.8</code> <code>ASP.NET Core 8</code> <code>SQL Server</code> <code>ADO.NET</code></p>
    </td>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/muriloai/healthcare-claims-api">Healthcare Claims API</a></h4>
      <p>API RESTful para validação, emissão e liquidação de guias médicas em operadoras de saúde, projetada para evitar glosas por falhas de elegibilidade (vigência do plano, carência e credenciamento ativo). Implementa isolamento de recursos por prestador autenticado (<em>resource hiding</em> para resguardar o sigilo entre clínicas) e padroniza respostas de falha no formato internacional RFC 9457 (<em>Problem Details</em>), sem expor dados internos.</p>
      <p><strong>Stack:</strong> <code>C#</code> <code>.NET 10</code> <code>Minimal APIs</code> <code>EF Core</code> <code>SQLite</code> <code>MSTest</code></p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/muriloai/order-orchestrator">Order Orchestrator</a></h4>
      <p>Arquitetura orientada a eventos para processamento distribuído de pedidos e baixa assíncrona de estoque, desacoplando a API de recepção do worker de inventário. Trata problemas comuns em ambientes distribuídos, como reentrega de mensagens pelo broker e deduplicação idempotente para impedir baixas repetidas de saldo, contando com painel em Angular e rastreamento ponta a ponta via OpenTelemetry e Jaeger.</p>
      <p><strong>Stack:</strong> <code>C# 14</code> <code>.NET 10</code> <code>Angular</code> <code>RabbitMQ</code> <code>SQL Server</code> <code>SignalR</code> <code>OpenTelemetry</code></p>
    </td>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/muriloai/gestao-orcamentos-razor-sqlserver">Gestão de Orçamentos</a></h4>
      <p>Aplicação web para cadastro de clientes e controle do ciclo comercial de propostas, do rascunho à aprovação ou recusa. Garante que os valores e condições enviados ao cliente permaneçam preservados no histórico da proposta mesmo quando o cadastro original sofre alterações posteriores, além de incluir monitoramento de vencimentos em segundo plano, consulta de endereço via ViaCEP e API JSON.</p>
      <p><strong>Stack:</strong> <code>C#</code> <code>ASP.NET Core 10</code> <code>Razor / MVC</code> <code>EF Core</code> <code>SQL Server</code></p>
    </td>
  </tr>
</table>

#### Aplicações Desktop, Segurança e Relatórios Corporativos

<table>
  <tr>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/muriloai/NetStatAnalyzer">NetStatAnalyzer</a></h4>
      <p>Ferramenta de segurança e monitoramento em tempo real para estações Windows corporativas (<a href="https://github.com/muriloai/NetStatAnalyzer/releases">v1.3.0</a>, com 52 testes automatizados). Integra-se às APIs nativas Win32 para mapear conexões TCP/UDP, taxas de I/O de rede e consumo de CPU por processo, além de auditar o Agendador de Tarefas e o Registro do Windows em busca de proxies residenciais, mineração não autorizada e scripts PowerShell ocultos.</p>
      <p><strong>Stack:</strong> <code>C#</code> <code>.NET 8 (Windows)</code> <code>WPF</code> <code>Win32 API</code> <code>xUnit</code></p>
    </td>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/muriloai/winforms-survey-data-entry">Survey Data Entry</a></h4>
      <p>Sistema desktop para estruturação de formulários, coleta rápida via teclado em postos de atendimento e tabulação estatística de pesquisas. O repositório inclui a <a href="https://github.com/muriloai/winforms-survey-data-entry/blob/main/HISTORIA.md">memória técnica de 2014 a 2026</a>, mostrando a migração do servidor MySQL externo para SQLite local auto-inicializado, a blindagem das consultas com parâmetros e transações ACID e a reformulação visual da interface.</p>
      <p><strong>Stack:</strong> <code>C#</code> <code>Windows Forms</code> <code>.NET Framework</code> <code>SQLite</code> <code>ACID</code></p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/muriloai/CoreSearch">Core Search</a></h4>
      <p>Utilitário desktop leve para busca textual dentro de arquivos de código-fonte e logs no Windows, suprindo a limitação padrão do Explorer sem depender de indexação pesada no sistema. Realiza leitura sob demanda linha a linha (<code>StreamReader</code>) para inspecionar arquivos de múltiplos gigabytes sem estourar a memória RAM, ignorando bloqueios de permissão ou arquivos em uso e mantendo a interface responsiva com cancelamento instantâneo.</p>
      <p><strong>Stack:</strong> <code>C#</code> <code>.NET 8</code> <code>WPF</code> <code>MVVM</code> <code>Clean Architecture</code></p>
    </td>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/muriloai/crystal-reports-service-billing">Service Billing | Crystal Reports</a></h4>
      <p>Projeto de relatórios corporativos de faturamento, liquidação financeira e contas a receber desenvolvidos no SAP Crystal Reports 2020 e conectados ao PostgreSQL via ODBC de 64 bits. Contempla a modelagem relacional do ciclo de vendas e distribuição atacadista, views analíticas de consolidação por data de corte e regras para apuração de saldos em aberto, amortizações e faixas de atraso (<em>aging</em>).</p>
      <p><strong>Stack:</strong> <code>SAP Crystal Reports 2020</code> <code>PostgreSQL</code> <code>SQL</code> <code>ODBC x64</code></p>
    </td>
  </tr>
</table>

#### Laboratórios de Modernização (Legado vs. Plataforma Atual)

<table>
  <tr>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/muriloai/dotnet-modernization-lab">.NET Modernization Lab</a></h4>
      <p>Laboratório prático com <strong>25 conceitos isolados</strong> comparando, lado a lado, implementações equivalentes no <strong>.NET Framework 4.8.1 (C# 7.3)</strong> e no <strong>.NET 10 (C# 14)</strong>. Cada módulo traz dois projetos independentes e funcionais cobrindo estrutura de host, injeção de dependência, autenticação, EF6 vs. EF Core, Minimal APIs, <code>IHttpClientFactory</code>, SignalR, tratamento de erros com Problem Details, cache e <code>Span&lt;T&gt;</code>.</p>
      <p><strong>Stack:</strong> <code>C# 7.3 → 14</code> <code>.NET Framework 4.8.1</code> <code>.NET 10</code> <code>ASP.NET Core</code></p>
    </td>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/muriloai/angular-modernization-lab">Angular Modernization Lab</a></h4>
      <p>Catálogo prático com <strong>40 conceitos isolados</strong> comparando o modelo clássico do <strong>Angular 15</strong> (<code>NgModule</code>, <code>Zone.js</code>, RxJS obrigatório e Webpack) com a arquitetura moderna do <strong>Angular 22</strong> (componentes <em>Standalone</em>, <em>Signals</em>, execução <em>Zoneless</em>, Vite/esbuild e <em>Resource API</em>), acompanhado de guias consolidados e dicionário rápido de migração (<em>"De → Para"</em>).</p>
      <p><strong>Stack:</strong> <code>Angular 15 → 22</code> <code>TypeScript</code> <code>Signals</code> <code>Standalone</code> <code>RxJS</code></p>
    </td>
  </tr>
</table>

<p align="right">
  <a href="https://github.com/muriloai?tab=repositories"><strong>Ver todos os repositórios públicos →</strong></a>
</p>

---

### Tecnologias

#### No trabalho e produção
*O que uso no dia a dia corporativo:*

<p align="left">
  <img height="36" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/csharp/csharp-original.svg" alt="C#" title="C#" />
  <img height="36" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/dot-net/dot-net-original.svg" alt=".NET" title=".NET" />
  <img height="36" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/angularjs/angularjs-original.svg" alt="Angular" title="Angular" />
  <img height="36" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/typescript/typescript-original.svg" alt="TypeScript" title="TypeScript" />
  <img height="36" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="JavaScript" title="JavaScript" />
  <img height="36" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/microsoftsqlserver/microsoftsqlserver-plain.svg" alt="SQL Server" title="SQL Server" />
    <img height="36" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/githubactions/githubactions-original.svg" alt="GitHub Actions" title="GitHub Actions" />
  <img height="36" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/sass/sass-original.svg" alt="Sass/SCSS" title="Sass/SCSS" />
  <img height="36" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/git/git-original.svg" alt="Git" title="Git" />
  <img height="36" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/azure/azure-original.svg" alt="Azure DevOps" title="Azure DevOps" />
</p>

#### Projetos próprios (DXS)
*Ferramentas que crio e mantenho:*

<p align="left">
  <img height="36" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/astro/astro-original.svg" alt="Astro" title="Astro" />
  <img height="36" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/chrome/chrome-original.svg" alt="Chrome Extensions" title="Chrome Extensions" />
  <img height="36" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/php/php-original.svg" alt="PHP" title="PHP" />
  <img height="36" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original.svg" alt="MySQL" title="MySQL" />
</p>

* **Extensões para o Chrome:** Ferramentas publicadas na Chrome Web Store.
* **Ferramentas web com privacidade:** Utilitários para editores e devs que processam tudo direto no navegador, com total privacidade confirmada, sem coletar dados do usuário.
* **Sites estáticos rápidos:** Páginas feitas com Astro e deploy automático via GitHub Actions.

#### Estudos e aprofundamento
*O que venho estudando e praticando:*

<p align="left">
  <img height="36" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/azure/azure-original.svg" alt="Azure" title="Microsoft Azure" />
  <img height="36" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/docker/docker-original.svg" alt="Docker" title="Docker" />
</p>

* Tenho certificação **Microsoft Certified: Azure Fundamentals (AZ-900)**.
* Estou aprofundando em Docker, mensageria e nas versões mais recentes do .NET e do Angular.
* Formação: Análise e Desenvolvimento de Sistemas e pós-graduação em Big Data Analytics.

---

### Estatísticas

<div align="center">
  <a href="https://github.com/muriloai">
    <img src="https://github-readme-stats-git-master-muriloabrs-projects.vercel.app/api?username=muriloai&show_icons=true&theme=github_dark&bg_color=0d1117&hide_border=true&include_all_commits=true&count_private=true" alt="Estatísticas do GitHub" height="145" />
    <img src="https://github-readme-stats-git-master-muriloabrs-projects.vercel.app/api/top-langs/?username=muriloai&layout=compact&theme=github_dark&bg_color=0d1117&hide_border=true&langs_count=8&custom_title=Linguagens%20Mais%20Usadas" alt="Linguagens Mais Usadas" height="145" />
  </a>
</div>

---

### Onde me encontrar

<div align="center">
  <a href="https://www.linkedin.com/in/muriloabreuinacio" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="https://dataxstudios.com.br" target="_blank">
    <img src="https://img.shields.io/badge/Site-DataXStudios-0052CC?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Site Oficial" />
  </a> 
  <a href="mailto:contato@dataxstudios.com.br"> 
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /> 
  </a> 
</div>
