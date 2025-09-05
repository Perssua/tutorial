# Chave de API do OpenRouter

## Visão Geral
O Perssua pode se conectar ao **OpenRouter**, um provedor de modelos de IA via API. Para isso, você precisa gerar e adicionar sua própria **chave de API do OpenRouter**.  
Este guia explica como criar a chave, onde inseri-la no Perssua e quais limitações considerar.

---

## Pré-requisitos
- Uma **conta no OpenRouter** (cadastre-se em [https://openrouter.ai](https://openrouter.ai)).  
- Entendimento básico sobre chaves de API: funcionam como senhas — mantenha-as em segredo e nunca compartilhe publicamente.  
- Perssua instalado e ativo.

---

## Passo a passo — Gerar uma chave de API do OpenRouter
1. Acesse [https://openrouter.ai/keys](https://openrouter.ai/keys) e faça login.  
2. Clique em **Create Key**.  
3. Dê um nome descritivo para a chave (ex: *Integração Perssua*).  
4. Copie a string gerada (começa com `sk-...`).  
   - **Importante:** você só verá essa chave uma vez. Guarde em local seguro.  
5. No Perssua, vá em **Configurações → Integrações → OpenRouter**.  
6. Cole a chave no campo **API Key**.  
7. Salve as alterações e teste enviando um prompt curto pelo chat.

---

## Limitações & Observações
- **Cotas de uso:**  
  - Contas gratuitas do OpenRouter têm limite de requisições. Veja [preços do OpenRouter](https://openrouter.ai/pricing) para detalhes.  
  - Ao exceder a cota, as requisições falham até você fazer upgrade ou adicionar créditos.  
- **Disponibilidade de modelos:**  
  - Nem todos os modelos do OpenRouter podem estar disponíveis no Perssua.  
  - Alguns modelos premium exigem pagamento direto no OpenRouter.  
- **Latência:**  
  - O tempo de resposta pode variar conforme o modelo/provedor.  
- **Segurança:**  
  - Chaves de API são sensíveis — trate como senhas.  
  - Troque a chave se for comprometida ou não for mais necessária.  
- **Planos do Perssua:**  
  - Usar sua própria chave de API **não** remove os limites do seu plano Perssua (ex: máximo de screenshots no plano gratuito).  

---

## Atalhos
Não há atalho dedicado para gerenciar chaves de API.  
Atalhos relacionados para testar prompts após integração:  
- **Ctrl + D** — Gravar & transcrever áudio (Whisper).  
- **Ctrl + E** — Capturar screenshot.  
- **Ctrl + Enter** — Analisar o último screenshot.  
- **Ctrl + B** — Alternar visibilidade do app.  

---

## Dicas
- Use **chaves separadas** para cada app/projeto para melhor controle.  
- Guarde suas chaves em um gerenciador de senhas seguro.  
- Monitore o painel do OpenRouter para uso e cobrança.  

## Solução de Problemas
- **Erro “Invalid key”:** confira se não há espaços extras ao colar.  
- **Sem resposta:** verifique sua cota no OpenRouter e a conexão do Perssua com a internet.  
- **Modelo errado retornado:** selecione um modelo suportado nas configurações do Perssua.