# 🧠 MCPMultAgent — Agentes Inteligentes com Model Context Protocol (MCP)

## 💡 Visão Geral

Este projeto foi desenvolvido como parte dos estudos do curso [MCP na Prática: Crie Agentes LLM Conectados e Inteligentes](https://www.udemy.com/course/mcp-na-pratica-crie-agentes-llm-conectados-e-inteligente) na Udemy, ministrado por Fernando Amaral e Rodrigo Amaral.

O objetivo é construir agentes inteligentes baseados em **LLMs (Large Language Models)** que se comunicam entre si e com o ambiente por meio do **Model Context Protocol (MCP)** — um protocolo leve e moderno que permite orquestrar interações entre modelos de linguagem, ferramentas externas e dados estruturados.

Este projeto simula um ambiente multiagente onde cada agente pode acessar ferramentas, executar ações, consultar dados e interagir com o usuário de forma estruturada e útil.

---

## 🧠 Conceitos Aplicados

- **MCP (Model Context Protocol)**: protocolo que define como agentes compartilham contexto, estado e ferramentas.
- **LLMs**: modelos de linguagem que interpretam comandos e geram respostas inteligentes.
- **Tools**: ferramentas que os agentes podem utilizar para acessar dados, executar funções ou interagir com APIs.
- **Resources**: fontes de dados que os agentes podem consultar.
- **Prompts**: instruções que guiam o comportamento dos agentes.

---

## 🛠️ Tecnologias Utilizadas

- `Python`  
- `LangChain`  
- `OpenAI API`  
- `Streamlit` (opcional para interface)  
- `dotenv` para variáveis de ambiente  
- `MCP` (estrutura personalizada)

---

## 🚀 Primeiros Passos

### ✅ Pré-requisitos
- Python 3.10+
- pip
- Chave de API (OpenAI ou outro provedor LLM)

### 📦 Instalação e Ambiente Virtual

```bash
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
```
Configure o arquivo .env com sua chave de API:
```env
OPENAI_API_KEY=sk-xxxxxxxxxxxxxxxxxxxx
```

### ▶️ Executando o Projeto
```Bash
python main.py
```
Ou, se houver interface web:
```Bash
streamlit run app.py
```


## 📁 Estrutura do Projeto
```
MCPMultAgent/
├── main.py               # Execução principal
├── mcp/                  # Implementação do protocolo MCP
│   ├── agent.py          # Lógica de agente
│   ├── server.py         # Servidor MCP
│   └── client.py         # Cliente MCP
├── tools/                # Ferramentas disponíveis para os agentes
├── .env                  # Chave de API
├── requirements.txt      # Dependências
└── README.md  
```

## 📚 Aprendizados
- Criação de agentes LLM conectados com ferramentas reais
- Implementação de servidores e clientes MCP
- Integração de modelos de linguagem com dados e APIs
- Construção de interfaces conversacionais com Streamlit
- Orquestração de múltiplos agentes em um sistema distribuído

## 🔮 Próximos Passos
- Adicionar novos agentes com especializações distintas
- Expandir o conjunto de ferramentas disponíveis
- Criar simulações de tomada de decisão colaborativa
- Testar integração com CrewAI e LangGraph

## 👩‍💻 Autora

Aline Assunção

Engenheira de Qualidade em transição para Inteligência Artificial

📫 [LinkedIn](https://www.linkedin.com/in/alineassuncaoai/)  

📬 aline.jassuncao@gmail.com

>_"Agentes inteligentes não apenas respondem — eles se conectam, colaboram e agem."_
