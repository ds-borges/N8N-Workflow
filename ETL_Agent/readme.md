# Projetos de Agentes Autônomos (ETL com IA) 🤖

Bem-vindo à central dos meus projetos de Agentes Autônomos! Este repositório contém uma coleção de agentes de software desenvolvidos para automatizar tarefas de ETL (Extração, Transformação e Carga), funcionando como assistentes pessoais inteligentes.

Cada agente utiliza conceitos de IA e se conecta a diferentes serviços para executar tarefas que vão desde a organização de e-mails até o gerenciamento de dados em um banco de dados.

## 🛠️ Tecnologias Principais

Estes projetos combinam diversas ferramentas para criar fluxos de automação robustos e eficientes:

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![n8n](https://img.shields.io/badge/n8n-12B57F?style=for-the-badge&logo=n8n&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)
![Google Calendar](https://img.shields.io/badge/Google_Calendar-4285F4?style=for-the-badge&logo=googlecalendar&logoColor=white)
![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)
![Telegram](https://img.shields.io/badge/Telegram-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)

---

## 🧩 Shared-components

Esta pasta contém arquivos que servem como base para múltiplos agentes, garantindo a reutilização de código e a padronização das operações.

| Arquivo | Descrição | Agentes Dependentes |
| :--- | :--- | :--- |
| `querry_executor_sql.json` | Contém a lógica central para executar consultas SQL, servindo como uma base para todas as interações com o banco de dados. | `Books-agent`, `Financial-monitoring` |

---

## 🤖 Nossos Agentes em Ação

Abaixo está a descrição de cada agente desenvolvido até o momento. Cada título corresponde a uma pasta no repositório.

### 📚 Books-agent
Um agente criado para gerenciar uma coleção de livros de forma simples e direta, conectando-se a um banco de dados na nuvem.

* **Contexto:** Este projeto foi desenvolvido para auxiliar uma professora de Jardim de Infância de uma escola municipal a organizar os livros da sua turma.
* **Funcionalidades:**
    * Adicionar novos livros ao banco de dados.
    * Consultar a lista de livros existentes e suas informações.
    * Remover livros do registro.
* **Tecnologias:** Supabase (utiliza `Shared-components/querry_executor_sql.json`).

### 📧 Email-classifier
Este agente funciona como um assistente pessoal que lê e classifica e-mails recebidos, tomando ações para organizar a agenda e a caixa de entrada do usuário.

* **Funcionalidades:**
    * **Categoria `Estudo`:** Agenda automaticamente eventos, lives e aulas no Google Calendar.
    * **Categoria `Finanças`:** Marca datas de pagamento de cobranças no calendário.
    * **Categorias `Itens Salvos` e `Arquivo Morto`:** Marcam os e-mails correspondentes como lidos para limpar a caixa de entrada.
* **Tecnologias:** Google Calendar API.

### 💬 Instagram-agent
Um agente de conversação projetado para automatizar o atendimento via Direct Messages (DMs) no Instagram, com foco em vendas e prospecção.

* **Funcionalidades:**
    * Responde a mensagens de novos seguidores ou clientes.
    * Apresenta e vende um curso de automação com n8n.
    * Agenda reuniões de negócios diretamente no calendário.
* **Tecnologias:** Instagram API, Google Calendar API, n8n.

### 💰 Financial-monitoring
Este agente automatiza o registro e a consulta de informações financeiras, interagindo com o usuário através de plataformas de mensagens.

* **Funcionalidades:**
    * Recebe e armazena dados de contas e despesas em um banco de dados.
    * Permite ao usuário consultar os dados armazenados.
    * Permite a remoção de registros financeiros.
* **Tecnologias:** Supabase, Telegram (utiliza `Shared-components/querry_executor_sql.json`).

### 📄 Summary-Agent
Um agente focado em processamento de conteúdo, capaz de extrair e resumir informações de documentos.

* **Funcionalidades:**
    * Realiza o upload de livros ou documentos para um banco de dados.
    * Extrai, converte e processa o conteúdo do arquivo.
    * Gera resumos e apresenta informações relevantes sobre o assunto ao usuário.
* **Tecnologias:** Supabase.

## Author

**Diego Sousa Borges**

* **LinkedIn:** [in/ds-borges](https://www.linkedin.com/in/ds-borges/)
* **GitHub:** [ds-borges](https://github.com/ds-borges)