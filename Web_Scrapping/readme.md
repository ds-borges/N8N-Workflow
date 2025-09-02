# Agentes de Web Scraping e Automação 🌐

Bem-vindo à seção de projetos focados em Web Scraping e automação de tarefas. Os agentes neste diretório são projetados para extrair informações de sites e APIs na internet, processar esses dados com Inteligência Artificial e entregar insights úteis através de canais de mensagens como Telegram e WhatsApp.

## 🛠️ Tecnologias Principais

Estes workflows foram construídos utilizando um ecossistema de ferramentas modernas para orquestração, IA e comunicação.

![n8n](https://img.shields.io/badge/n8n-12B57F?style=for-the-badge&logo=n8n&logoColor=white)
![Google Gemini](https://img.shields.io/badge/Google_Gemini-8E77F0?style=for-the-badge&logo=googlegemini&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![WhatsApp](https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)
![Telegram](https://img.shields.io/badge/Telegram-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)

---

## 🚀 Nossos Agentes em Ação

Abaixo estão os detalhes de cada workflow de automação.

### 📰 Newsletter_agent.json
Um agente que cria um boletim informativo diário e imparcial, resumindo a principal notícia de política de um grande portal de notícias brasileiro.

* **Objetivo:** Manter o usuário informado com um resumo rápido e direto da notícia política mais recente, escolhendo a fonte de forma aleatória para evitar viés.
* **Fluxo de Trabalho:**
    1.  **Disparo Diário:** O workflow é iniciado automaticamente em um horário agendado.
    2.  **Seleção Aleatória de Portal:** O agente escolhe um site de uma lista pré-definida: `Gazeta do Povo`, `Poder360`, `CartaCapital`, `Revista Oeste` ou `IstoÉ Dinheiro`.
    3.  **Scraping da Notícia:** Acessa o portal selecionado e extrai o link da notícia mais recente sobre política.
    4.  **Resumo com IA:** O conteúdo da notícia é processado pelo Google Gemini para gerar um resumo conciso.
    5.  **Envio Multicanal:** O resumo final é enviado para o usuário via Telegram e WhatsApp.

### ☀️ Weather_agent.json
Um agente que envia um relatório meteorológico matinal personalizado para a cidade de Jataí - GO.

* **Objetivo:** Fornecer informações úteis sobre o tempo local no início do dia, de forma automatizada.
* **Fluxo de Trabalho:**
    1.  **Disparo Agendado:** O workflow é ativado automaticamente todas as manhãs.
    2.  **Coleta de Dados:** Conecta-se à API do **OpenWeatherMap** para obter os dados meteorológicos de Jataí.
    3.  **Geração da Mensagem com IA:** Utiliza o Google Gemini para criar uma mensagem amigável contendo:
        * Temperatura atual e previsão.
        * Umidade do ar.
        * Horário do nascer e do pôr do sol.
    4.  **Envio para Mensageiros:** A previsão do tempo é enviada para o Telegram e WhatsApp.

### 🎓 Simple_WebScraping-Jornada_de_Dados
Um agente de chat, desenvolvido como projeto de aula, que responde a perguntas sobre o site "Sua Jornada de Dados".

* **Objetivo:** Demonstrar um agente de IA com ferramenta de web scraping em tempo real para responder perguntas factuais com base no conteúdo de um site específico.
* **Fluxo de Trabalho:**
    1.  **Ativação por Chat:** O agente é ativado quando recebe uma mensagem do usuário.
    2.  **Scraping em Tempo Real:** Acessa o site `suajornadadedados.com.br` para buscar a informação solicitada.
    3.  **Resposta Estruturada com IA:** O Google Gemini processa a informação coletada e responde seguindo regras estritas:
        * Inicia a resposta com "Pesquisa realizada em: [data atual]".
        * Retorna apenas as 3 informações mais relevantes.
        * Nunca inventa respostas, baseando-se 100% no conteúdo do site.

## Author

**Diego Sousa Borges**

* **LinkedIn:** [in/ds-borges](https://www.linkedin.com/in/ds-borges/)
* **GitHub:** [ds-borges](https://github.com/ds-borges)