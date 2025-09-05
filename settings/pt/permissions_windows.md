
# Permissões do Windows

## Visão Geral
O Perssua precisa de algumas **permissões do Windows** para capturar sua tela, gravar áudio e exibir notificações.  
Sem essas permissões, recursos como **Captura de Screenshot (Ctrl + E)** ou **Whisper (Ctrl + D)** não funcionarão.

Este guia explica **por que** precisamos dessas permissões e como concedê-las passo a passo.

---

## Por que as permissões são necessárias
- **Screen Capture:** Necessário para o Perssua capturar screenshots dos seus apps/janelas para análise. O Windows controla isso para proteger sua privacidade.  
- **Microphone:** Necessário para o Whisper e outros recursos de áudio (Ctrl + D). Sem isso, o Perssua não pode transcrever fala.  
- **Notifications:** Necessário para o Perssua exibir notificações do sistema (ex: análise concluída).  
- **Background Apps (opcional):** Permite que o Perssua continue ouvindo atalhos mesmo minimizado.

---

## Passos — Como conceder permissões no Windows

### Ativar Screen Capture
1. Abra **Settings → Privacy & security**.  
2. Vá até **App permissions → Camera & screen capture** (pode variar conforme a versão do Windows).  
3. Certifique-se de que **Allow desktop apps to capture your screen** está ativado (**On**).  
4. Verifique se o **Perssua** está listado e ativado.

### Ativar Microphone
1. Vá em **Settings → Privacy & security → Microphone**.  
2. Ative **Microphone access** (**On**).  
3. Em **Let desktop apps access your microphone**, deixe em **On**.  
4. Certifique-se de que o **Perssua** aparece na lista com acesso permitido.

### Ativar Notifications
1. Vá em **Settings → System → Notifications**.  
2. Localize o **Perssua** na lista de apps.  
3. Ative as notificações (**On**).  
4. Opcionalmente, personalize o estilo das notificações (banner, som, prioridade).

### Permitir Background Apps (opcional)
1. Abra **Settings → Apps → Installed apps**.  
2. Selecione **Perssua → Advanced options**.  
3. Em **Background apps permissions**, escolha **Let this app run in background**.

---

## Atalhos para testar após conceder permissões
- **Ctrl + E** — Capturar screenshot (requer Screen Capture).  
- **Ctrl + Enter** — Analisar o screenshot mais recente.  
- **Ctrl + D** — Gravar & transcrever áudio (requer Microphone).  
- **Ctrl + B** — Alternar visibilidade do app (requer permissão de background para atalhos globais).  
- **Ctrl + Up/Down** — Rolar o chat do Perssua.

---

## Dicas
- Após alterar permissões, reinicie o Perssua para aplicar as mudanças.  
- Se as permissões não aparecerem na lista, tente acionar o recurso uma vez (ex: tente capturar um screenshot) para o Windows solicitar.  
- Use o atalho **Windows + I** para abrir rapidamente o **Settings**.

## Solução de Problemas
