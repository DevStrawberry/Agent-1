# Agent-1
### 📦 Projeto: Agente de IA com chat + execução local

---

# 🗂 Estrutura do projeto
```
/ia-agent/
├── backend/
│   ├── main.py
│   ├── requirements.txt
│   └── .env
└── frontend/
    ├── App.js
    └── package.json
```

---

# 🚀 Como rodar o projeto

## 🔧 Backend (Python + FastAPI)

1️⃣ Acesse a pasta backend:
```bash
cd backend
```

2️⃣ Instale as dependências:
```bash
pip install -r requirements.txt
```

3️⃣ Configure o arquivo `.env` com sua chave da OpenAI:
```
OPENAI_API_KEY=your_openai_api_key_here
```

4️⃣ Rode o servidor local:
```bash
uvicorn main:app --reload --host 0.0.0.0 --port 8000
```

---

## 📱 Frontend (React Native + Expo)

1️⃣ Acesse a pasta frontend:
```bash
cd frontend
```

2️⃣ Instale as dependências:
```bash
npm install
```

3️⃣ Inicie o projeto com Expo:
```bash
npx expo start
```

4️⃣ Use o app **Expo Go** no seu celular para escanear o QR Code e abrir o app.

⚠ **Importante:** No arquivo `App.js`, ajuste o endpoint para o IP correto do backend:
```js
fetch('http://<backend-ip>:8000/ask', ...)
```
Por exemplo: `http://192.168.0.100:8000/ask`

---

# ✨ O que está pronto
✅ Backend FastAPI conectando com GPT-4 API da OpenAI.  
✅ Frontend React Native (Expo) com tela de chat simples.  
✅ Comunicação completa entre app e backend.  
✅ Execução local de ações simples (ex: criar arquivo).  

---

# 📌 Próximos passos (sugestões)
- Melhorar interface do app com componentes visuais (React Native Paper ou NativeBase).
- Adicionar autenticação de usuário.
- Implementar histórico salvo no backend.
- Expandir os comandos locais: abrir arquivos, listar diretórios, executar scripts.
- Conectar a serviços externos (Google Calendar, Email, Notion etc).

---
