# Whisper

## Visão Geral
O Whisper transcreve sua voz e pode enviar as transcrições para a IA. Use o **modo manual** para capturar sob demanda ou o **modo automático** para transcrever e enviar a cada _N_ segundos. Sempre teste com um exemplo curto antes de usar ao vivo.

## Pré-requisitos
- Microfone funcionando, conectado e selecionado no app.
- Permissões do sistema concedidas (Microphone; no Windows/macOS, permita o acesso do app ao áudio).
- Conexão de internet estável.

## Passos

### Manual (sob demanda)
1. Abra **Features → Whisper**.
2. Clique no ícone de **Microphone** **ou pressione `Ctrl + D`** para capturar a fala.
3. Revise a transcrição e **clique em _Send to AI_**.
4. Leia a resposta no painel de chat.

### Automático (a cada N segundos)
1. Abra **Features → Whisper**.
2. Ative o **Auto Transcribe**.
3. Defina o **Interval** (ex: **10s**).
4. Ative o **Auto-send to AI** (se disponível) para enviar cada trecho automaticamente.
5. Acompanhe as transcrições e respostas no chat.

## Configurações de Áudio
- **Input device:** Escolha o microfone correto em **Settings → Audio**.
- **Input level / gain:** Ajuste para que a fala normal não ultrapasse o limite.
- **Noise suppression:** Ative para reduzir ruído de fundo.
- **Echo cancellation (se disponível):** Útil ao usar alto-falantes em vez de fones.
- **Language (opcional):** Selecione seu idioma principal para melhor precisão.

## Atalhos
- **`Ctrl + D`** — Gravar & transcrever áudio (captura manual).
- Relacionados (workflow opcional):
  - **`Ctrl + E`** — Capturar screenshot.
  - **`Ctrl + Enter`** — Analisar o screenshot mais recente.

## Dicas
- Transcrição contínua pode consumir créditos — use intervalos sensatos (ex: 10–20s).
- Para melhor precisão, fale próximo ao microfone e reduza ruídos no ambiente.
- Use fones de ouvido para evitar eco em chamadas.

## Solução de Problemas
- **Nenhuma entrada detectada:** Selecione o microfone correto e confira as permissões do sistema.
- **Baixa precisão:** Confirme o idioma e reduza ruídos.
- **Delays ou falhas:** Reduza o intervalo, feche apps pesados ou melhore a conexão.
- **Clipping/distorção:** Reduza o ganho em **Settings → Audio**.
