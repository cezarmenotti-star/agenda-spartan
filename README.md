# 📅 Agenda Compartilhável com Firebase

Sincronização em tempo real para agendamentos de reuniões.

## ✨ Características

- 📅 Calendário visual interativo
- 🔒 Modo proprietário (bloquear horários)
- 👥 Modo vendedor (agendar reuniões)
- 🔴 Cores por tipo de reunião (Online, Interno, Externo, Entrevista)
- ⚡ Sincronização em tempo real com Firebase
- 📱 Totalmente responsivo (desktop e mobile)

## 🚀 Começar Rápido

### 1. Instalar Dependências

```bash
npm install
```

### 2. Configurar Credenciais Firebase

Renomeie `config-template.js` para `config.js` e adicione suas credenciais:

```javascript
export const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_AUTH_DOMAIN",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_STORAGE_BUCKET",
  messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
  appId: "YOUR_APP_ID",
  databaseURL: "YOUR_DATABASE_URL"
};
```

### 3. Executar Localmente

```bash
npm start
```

Acesse: **http://localhost:8080**

## 👨‍💼 Modo Proprietário

- Ver calendário completo
- Bloquear horários indisponíveis
- Visualizar todas as reuniões agendadas
- Deletar agendamentos

## 👥 Modo Vendedor

- Visualizar horários disponíveis
- Agendar reuniões
- Preencher informações:
  - Consultor
  - Nome do Cliente
  - Email
  - Formato da Reunião (Online, Interno, Externo, Entrevista)
  - Detalhes/Notas

## 🎨 Cores das Reuniões

- 🔵 **Online** - Azul
- 🔴 **Interno** - Vermelho
- 🟢 **Externo** - Verde
- 🟣 **Entrevista** - Roxo

## 🌐 Deploy

### Netlify

```bash
npm run deploy-netlify
```

### Firebase Hosting

```bash
npm run deploy-firebase
```

## 📁 Estrutura

```
agenda-compartilhavel/
├── index.html           # Aplicação completa
├── config.js            # Credenciais Firebase (gerar)
├── package.json         # Dependências
├── .gitignore          # Arquivos ignorados
└── README.md           # Este arquivo
```

## 🔐 Segurança

⚠️ **NUNCA** compartilhe seu `config.js` publicamente!

- Adicione `config.js` ao `.gitignore`
- Use variáveis de ambiente em produção
- Proteja suas credenciais do Firebase

## 📞 Suporte

Para questões sobre Firebase:
- Firebase Console: https://console.firebase.google.com
- Documentação: https://firebase.google.com/docs

## 📝 Licença

MIT

---

Desenvolvido com ❤️ para gerenciamento de agendamentos
