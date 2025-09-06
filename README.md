# Chatbot WhatsApp com IA - Versão Gratuita

Este é um chatbot para WhatsApp integrado com IA, desenvolvido para funcionar completamente de forma gratuita usando Hugging Face e Render.com.

## 🚀 Deploy Rápido

### 1. Fork este repositório no GitHub

### 2. Deploy no Render.com
1. Acesse [render.com](https://render.com) e faça login com GitHub
2. Clique em "New +" > "Web Service"
3. Conecte este repositório
4. Configure:
   - **Build Command**: `pip install -r requirements.txt`
   - **Start Command**: `python src/main.py`
   - **Environment**: Python 3

### 3. Configurar Variáveis de Ambiente
No painel do Render, adicione as seguintes variáveis:

```
WHATSAPP_TOKEN=seu_token_whatsapp_aqui
VERIFY_TOKEN=meu_token_verificacao_123
HUGGINGFACE_API_KEY=seu_token_huggingface_aqui
FLASK_ENV=production
```

### 4. Configurar Webhook no WhatsApp
1. Acesse [developers.facebook.com](https://developers.facebook.com)
2. Crie um app Business e adicione o produto WhatsApp
3. Configure o webhook:
   - **URL**: `https://seu-app.onrender.com/webhook`
   - **Verify Token**: `meu_token_verificacao_123`
   - **Subscribe to**: `messages`

## 🔧 Desenvolvimento Local

```bash
# Clonar o repositório
git clone <seu-repo>
cd chatbot-whatsapp

# Ativar ambiente virtual
source venv/bin/activate

# Instalar dependências
pip install -r requirements.txt

# Executar localmente
python src/main.py
```

## 📋 Funcionalidades

- ✅ Webhook para receber mensagens do WhatsApp
- ✅ Integração com Hugging Face (IA gratuita)
- ✅ Respostas pré-definidas para economizar API calls
- ✅ Logs detalhados para debugging
- ✅ Tratamento de erros robusto
- ✅ Deploy gratuito no Render.com

## 🔑 Obtendo as Credenciais

### WhatsApp Business API
1. Acesse [developers.facebook.com](https://developers.facebook.com)
2. Crie um app Business
3. Adicione o produto WhatsApp
4. Copie o token de acesso

### Hugging Face API
1. Acesse [huggingface.co](https://huggingface.co)
2. Crie uma conta gratuita
3. Vá em Settings > Access Tokens
4. Gere um token de leitura

## 💡 Dicas de Uso

- O plano gratuito do Render "dorme" após 15 minutos de inatividade
- A primeira resposta pode ser mais lenta devido ao "cold start"
- Use respostas pré-definidas para perguntas comuns
- Monitore os logs no painel do Render

## 🆘 Suporte

Se encontrar problemas:
1. Verifique os logs no painel do Render
2. Confirme se as variáveis de ambiente estão corretas
3. Teste o webhook usando o painel do WhatsApp Business

## 📊 Limites Gratuitos

- **Render.com**: 750 horas/mês (suficiente para uso contínuo)
- **Hugging Face**: Rate limits por hora
- **WhatsApp**: 1000 conversas/mês

---

**Custo total: R$ 0,00/mês** 🎉

