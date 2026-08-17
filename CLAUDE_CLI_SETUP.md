# 🤖 SETUP COM CLAUDE CODE CLI

Você baixou a pasta com toda a agenda pronta!

Agora falta apenas configurar o Firebase com seu Claude CLI.

---

## 📋 Passo 1: Baixar a Pasta

Você já tem em mãos:
- ✅ `index.html` (aplicação pronta)
- ✅ `config-template.js` (template de credenciais)
- ✅ `package.json` (dependências)
- ✅ `.gitignore` (segurança)
- ✅ `README.md` (documentação)

---

## 🔧 Passo 2: Usar Claude CLI para Automatizar

Seu Claude CLI tem acesso ao Firebase. Basta rodar:

```bash
cd agenda-compartilhavel
claude run "
1. Criar projeto Firebase chamado 'Agenda Consultores'
2. Ativar Realtime Database em modo Teste
3. Obter as 7 credenciais (apiKey, authDomain, projectId, storageBucket, messagingSenderId, appId, databaseURL)
4. Renomear config-template.js para config.js
5. Preencher as credenciais no config.js
"
```

---

## ⚡ Alternativa: Manual Rápido

Se preferir fazer manualmente:

### 1. Criar Projeto Firebase

```
https://console.firebase.google.com
→ Novo Projeto → Nome: "Agenda Consultores"
→ Próximo → Próximo → Criar Projeto
```

### 2. Ativar Realtime Database

```
Esquerda: Realtime Database
→ Criar Banco de Dados
→ Localização: Brasil (América do Sul)
→ Modo de Segurança: TESTE
→ Ativar
```

### 3. Copiar Credenciais

```
Configurações (⚙️) → Configurações do Projeto
→ Tab: Geral
→ Seus Apps → Web (</> ícone)
→ Registrar App → "agenda-web"
→ Copie o firebaseConfig
```

### 4. Preencher config.js

```bash
# Renomear o arquivo
mv config-template.js config.js

# Abrir em seu editor favorito e colar as credenciais
code config.js  # ou seu editor
```

---

## 🚀 Passo 3: Teste Localmente

```bash
npm install
npm start
```

Acesse: **http://localhost:8080**

Teste com 2 navegadores para ver a sincronização em tempo real! ✅

---

## 📤 Passo 4: Deploy (Opcional)

Quando pronto para compartilhar com consultores:

```bash
# Netlify (mais fácil)
npm run deploy-netlify

# Ou Firebase
npm run deploy-firebase
```

Você receberá um link público para compartilhar! 🎉

---

## ✅ Checklist

- [ ] Pasta baixada e aberta no terminal
- [ ] Firebase CLI usado ou projeto criado manualmente
- [ ] Credenciais obtidas do Firebase Console
- [ ] `config.js` preenchido com credenciais
- [ ] `npm install` executado
- [ ] `npm start` funcionando
- [ ] Testado em 2 navegadores (sincronização OK)
- [ ] Pronto para compartilhar com consultores!

---

## 🎯 Comandos Rápidos

```bash
# Entrar na pasta
cd agenda-compartilhavel

# Instalar dependências
npm install

# Rodar localmente
npm start

# Deploy em Netlify
npm run deploy-netlify

# Deploy em Firebase
npm run deploy-firebase
```

---

## 💡 Dicas

- Suas credenciais estão em `config.js` (nunca compartilhe!)
- Os dados são salvos no Firebase Realtime Database
- A aplicação funciona offline, sincroniza quando conecta
- Horários bloqueados aparecem com strikethrough
- Cores indicam tipo de reunião (Online, Interno, Externo, Entrevista)

---

## 🆘 Troubleshooting

**"npm: command not found"**
- Instale Node.js: https://nodejs.org

**"Porta 8080 já está em uso"**
```bash
npm start -- -p 3000  # Usar outra porta
```

**"Firebase não sincroniza"**
- Verifique se `config.js` está correto
- Confira as Regras de Segurança do Firebase

---

## 🎉 Pronto!

Sua agenda está pronta para usar!

Compartilhe o link com seus consultores e veja tudo sincronizar em tempo real! 🚀
