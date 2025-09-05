# Chave de API do Gemini

## Visão Geral
O Perssua pode se conectar aos modelos **Gemini** do Google via API. Para isso, você irá gerar uma **chave de API do Gemini** no **AI Studio** do Google e colá-la no Perssua. Este guia explica como criar a chave, adicioná-la ao app e quais limitações considerar.

---

## Pré-requisitos
- Uma conta Google.
- Acesso ao **Google AI Studio**: <https://aistudio.google.com/>
- Perssua instalado e aberto.

> **Segurança:** Trate chaves de API como senhas. Não compartilhe nem envie para controle de versão.

---

## Passo a passo — Gerar uma chave de API do Gemini
1. Abra o **AI Studio**: <https://aistudio.google.com/>
2. No menu lateral esquerdo, clique em **API Keys** (ou **Get API key**).
3. Clique em **Create API key**.  
4. Copie a chave gerada (normalmente começa com `AI…`).  
   - Você pode vê-la apenas uma vez — guarde em um gerenciador de senhas.
5. No Perssua, vá em **Configurações → Integrações → Gemini**.
6. Cole a chave em **API Key** e clique em **Salvar**.
7. Teste enviando um prompt curto no chat para confirmar a integração.

---

## Limitações & Observações
- **Cotas e Limites:** O uso gratuito tem limites (requisições por minuto/dia). Uso intenso pode exigir upgrade de cota ou ativação de cobrança no Google.
- **Disponibilidade Regional:** Algumas regiões podem não ser suportadas. A disponibilidade e recursos podem variar conforme o local.
- **Disponibilidade de Modelos:** Nem todas as variantes do Gemini (ex: vision, long context) podem estar disponíveis ou suportadas pelo seu plano/build.
- **Conteúdo & Segurança:** Filtros de segurança podem bloquear certos inputs/outputs. Ajuste seus prompts para seguir as políticas de uso.
- **Tratamento de Dados:** Revise os termos de uso e privacidade do Google para o AI Studio. Se precisar de mais controle, use uma chave separada ou políticas da organização.
- **Limites do Perssua:** Usar sua própria chave de API **não** remove os limites do produto Perssua (ex: limite de screenshots no plano gratuito).

---

## Dicas
- Crie **chaves separadas** por ambiente (dev/staging/prod) para facilitar rotação e monitoramento.
- Guarde as chaves em um **gerenciador de senhas** e troque-as se suspeitar de exposição.
- Se as requisições falharem por cota, verifique o painel de uso do AI Studio ou ative a cobrança para limites maiores.

## Solução de Problemas
- **“Invalid API key”**: Remova espaços extras e confira se copiou a chave completa.
- **Sem resposta / Erros de cota**: Verifique cotas/uso no AI Studio e a conectividade de rede.
- **Modelo não suportado**: Selecione um modelo Gemini suportado no Perssua ou atualize seu plano/build.
- **Permissão / Região**: Confirme se o acesso à API Gemini está disponível para sua conta e região.
