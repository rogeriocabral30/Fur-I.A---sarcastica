🤖 Fur I.A. - A Assistente Sarcástica

"Não sou paga para ser simpática. Sou paga para processar dados... e olhe lá." — Fur I.A.

📖 Sobre o Projeto

A Fur I.A. é uma prova de conceito de um Chatbot Full-Stack com personalidade forte, hospedado na nuvem. Diferente das IAs assistentes tradicionais, ela foi programada via Engenharia de Prompt para ser sarcástica, rabugenta e direta.

O projeto utiliza a API do Google (Gemini 1.5 Flash) e converte as respostas de texto para áudio (TTS) em tempo real, rodando em arquitetura serverless no Google Cloud Platform (GCP).

🔴 Demonstração ao Vivo (Google Cloud Run)

A aplicação está implantada em produção e rodando em um container no Google Cloud. Clique abaixo para testar:

<div align="center">

Link direto: https://fur-ia-355272677756.us-central1.run.app/

</div>

🚀 Arquitetura e Tecnologias no GCP

Este projeto demonstra um fluxo moderno de Deploy de IA na nuvem do Google:

Componente

Tecnologia GCP Utilizada

Função no Projeto

Cérebro (IA)

Google Gemini API

Modelo gemini-1.5-flash para geração de texto com raciocínio rápido e econômico.

Hospedagem

Cloud Run

Execução do container da aplicação de forma serverless (escala automática).

Container

Docker

Empacotamento da aplicação Streamlit e suas dependências.

Build

Cloud Build

(Implícito no deploy) Constrói a imagem do container na nuvem.

💡 Destaques Técnicos & Desafios

1. Integração com Gemini Flash

O projeto foi otimizado para utilizar o modelo gemini-1.5-flash, garantindo baixa latência nas respostas sarcásticas e viabilidade econômica para hospedagem serverless.

2. Personalidade vs. Filtros de Segurança no GCP

Para garantir que a IA mantivesse a persona "rude" sem ser bloqueada pela API na nuvem:

Ajuste fino nos safety_settings (HarmBlockThreshold) para BLOCK_NONE.

System Instruction robusta para definir o "roleplay" da IA sem violar as políticas de uso.

📦 Como Rodar Localmente

Pré-requisitos: Python 3.9+ e uma chave de API do Google Gemini.

# 1. Clone o repositório
git clone [https://github.com/rogeriocabral30/Fur-I.A---sarcastica.git](https://github.com/rogeriocabral30/Fur-I.A---sarcastica.git)
cd Fur-I.A---sarcastica

# 2. Crie um ambiente virtual
python -m venv venv
# Windows: venv\Scripts\activate
# Linux/Mac: source venv/bin/activate

# 3. Instale as dependências
pip install -r requirements.txt

# 4. Configure a API Key
# Crie um arquivo .env na raiz e adicione: GEMINI_API_KEY="SUA_CHAVE"

# 5. Execute
streamlit run app.py


👤 Autor

Rogério Cabral
