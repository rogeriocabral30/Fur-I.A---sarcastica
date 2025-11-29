# 🤖✨ Fur I.A. — A Assistente Sarcástica da Nuvem

<div align="center">

![Python](https://img.shields.io/badge/Python-3.9+-3776AB.svg?style=for-the-badge&logo=python&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B.svg?style=for-the-badge&logo=streamlit&logoColor=white)
![Google Gemini](https://img.shields.io/badge/Google_Gemini-8E75B2.svg?style=for-the-badge&logo=google&logoColor=white)
![Cloud Run](https://img.shields.io/badge/Google_Cloud_Run-4285F4.svg?style=for-the-badge&logo=google-cloud&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED.svg?style=for-the-badge&logo=docker&logoColor=white)

</div>

> 💬 *"Não sou paga para ser simpática. Sou paga para processar dados... e olhe lá."*  
> — **Fur I.A.**

---

## 📖 Sobre o Projeto

A **Fur I.A.** é um chatbot **Full-Stack** com personalidade forte — sarcástica, direta e levemente irritada com humanos.  
Ela foi construída com **Engenharia de Prompt**, hospedada em arquitetura **serverless** e equipada com:

- ✅ **Google Gemini 1.5 Flash**  
- ✅ **TTS em tempo real**  
- ✅ **Streamlit**  
- ✅ **Deploy automático no Cloud Run**

O resultado é uma IA que responde rápido, fala com você e ainda te trata mal — tudo com elegância.

---

## 🔴 Demonstração ao Vivo

Acesse a versão em produção no Google Cloud Run:

<div align="center">

[![Acessar Demo](https://img.shields.io/badge/▶️_CLIQUE_PARA_TESTAR-FF4B4B?style=for-the-badge&logo=google-cloud&logoColor=white)](https://fur-ia-355272677756.us-central1.run.app/)

**Link direto:**  
https://fur-ia-355272677756.us-central1.run.app/

</div>

---

## 🚀 Arquitetura e Tecnologias

| Componente | Tecnologia | Função |
|-----------|------------|--------|
| 🧠 **Cérebro da IA** | Google Gemini API | Modelo `gemini-1.5-flash` para respostas rápidas e econômicas |
| ☁️ **Hospedagem** | Cloud Run | Execução serverless com escala automática |
| 📦 **Container** | Docker | Empacotamento da aplicação |
| 🔧 **Build** | Cloud Build | Criação da imagem do container |

---

## 💡 Destaques Técnicos

### ✅ 1. Integração com Gemini Flash  
O modelo **gemini-1.5-flash** foi escolhido por:

- Baixa latência  
- Custo reduzido  
- Ótimo desempenho para diálogos rápidos e sarcásticos  

---

### ✅ 2. Personalidade vs. Filtros de Segurança  
Para manter a IA rude sem ser bloqueada:

- Ajuste fino em `safety_settings` → `BLOCK_NONE`  
- System Instruction reforçando o “roleplay”  
- Controle para não violar políticas da API  

---

### 📦 Como Rodar Localmente

Pré-requisitos: **Python 3.9+** e uma **API Key do Google Gemini**

## 1️⃣ Clone o repositório

bash
git clone https://github.com/rogeriocabral30/Fur-I.A---sarcastica.git
cd Fur-I.A---sarcastica

###  2️⃣ Crie um ambiente virtual
python -m venv venv

## 3️⃣ Instale as dependências
pip install -r requirements.txt

 4️⃣ Configure a API Key
 Crie um arquivo .env:
 GEMINI_API_KEY="SUA_CHAVE"

 5️⃣ Execute
streamlit run app.py


👨‍💻Autor — Rogério Cabral
<div align="left"><a href="https://www.linkedin.com/in/rogeriocabraldev/"><img src="https://img.shields.io/badge/LinkedIn-ACESSAR-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a>
<a href="https://github.com/rogeriocabral30"><img src="https://img.shields.io/badge/GitHub-ACESSAR-100000?style=for-the-badge&logo=github&logoColor=white"></a></div>

