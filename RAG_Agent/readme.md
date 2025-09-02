# Projetos com RAG (Retrieval-Augmented Generation) 🧠

Bem-vindo à seção de projetos que utilizam a técnica de RAG (Geração Aumentada por Recuperação). O objetivo aqui é criar agentes de IA especializados, capazes de responder perguntas com base em uma base de conhecimento privada e controlada.

Diferente de um chatbot genérico, um agente RAG consulta documentos específicos para fornecer respostas precisas, contextuais e confiáveis, reduzindo as chances de "alucinações".

## 🛠️ Tecnologias Principais

Para construir estes agentes, as seguintes tecnologias foram fundamentais, especialmente o banco de dados vetorial para a busca de informações.

![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![n8n](https://img.shields.io/badge/n8n-12B57F?style=for-the-badge&logo=n8n&logoColor=white)
---

## 🤔 Como Funciona o RAG?

O fluxo de trabalho de um agente RAG segue, de forma simplificada, os seguintes passos:

1.  **Indexação:** Os documentos da base de conhecimento (leis, editais, etc.) são processados e convertidos em vetores numéricos, que são armazenados em um banco de dados vetorial (Supabase Vector DB).
2.  **Pergunta:** O usuário envia uma pergunta para o agente.
3.  **Busca (Retrieval):** O sistema converte a pergunta em um vetor e busca no banco de dados os trechos de documentos mais relevantes ou semanticamente similares à pergunta.
4.  **Aumento (Augmentation):** Os trechos encontrados são combinados com a pergunta original, criando um prompt mais rico e contextualizado.
5.  **Geração (Generation):** Este prompt "aumentado" é enviado a um modelo de linguagem (LLM), que gera uma resposta precisa com base no contexto fornecido.

---

## 🚀 Nossos Agentes RAG

Abaixo estão os agentes desenvolvidos com a arquitetura RAG.

### ⚖️ Agente_RAG_Leis_Brasil
Um assistente jurídico virtual treinado para responder a perguntas com base nas principais leis do ordenamento jurídico brasileiro.

* **Objetivo:** Facilitar o acesso e a compreensão de informações legais, servindo como uma ferramenta de consulta rápida.
* **Base de Conhecimento:**
    * Constituição Federal
    * Código Civil
    * Consolidação das Leis do Trabalho (CLT)
    * Código de Defesa do Consumidor (CDC)
    * Lei Geral de Proteção de Dados Pessoais (LGPD)
* **Tecnologia-chave:** Supabase Vector DB para armazenar e consultar os vetores da legislação.

### 🎓 Agente_RAG_Universidade_Federal_De_Jatai
Um assistente acadêmico projetado para ajudar alunos e funcionários da Universidade Federal de Jataí (UFJ) a encontrar informações em documentos oficiais da instituição.

* **Objetivo:** Centralizar e simplificar o acesso a regulamentos e documentos importantes da universidade, respondendo a dúvidas comuns da comunidade acadêmica.
* **Base de Conhecimento:**
    * Documentos sobre a Colação de Grau.
    * Regulamentação Geral dos Cursos de Graduação.
    * Documento de apoio para o Projeto Final de Curso (TCC).
    * Edital de preenchimento de vagas remanescentes.
* **Tecnologia-chave:** Supabase Vector DB para indexar e realizar buscas nos documentos da UFJ.

## Author

**Diego Sousa Borges**

* **LinkedIn:** [in/ds-borges](https://www.linkedin.com/in/ds-borges/)
* **GitHub:** [ds-borges](https://github.com/ds-borges)