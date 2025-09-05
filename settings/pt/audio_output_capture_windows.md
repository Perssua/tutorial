# Captura de Áudio de Saída no Windows (Terceiros)

## Visão Geral
Este guia mostra como capturar o **áudio do sistema/saída** ("o que você ouve") no Windows usando um app de terceiros. Você pode rotear o áudio para o Perssua (dispositivo virtual) ou gravar/analisar externamente e enviar os resultados para o app.  
**Importante:** sempre teste com uma chamada curta ou reprodução de amostra antes de usar em produção e verifique as leis/políticas locais sobre gravação de áudio.

## Pré-requisitos
- Windows 10 ou 11 com direitos de administrador.
- Drivers de áudio atualizados.
- Permissão para gravar áudio quando necessário (empresa/conformidade).
- Um dos apps de terceiros abaixo instalado:
  - **Opção A (Roteamento):** [VB-Audio Virtual Cable] – cria um par virtual de saída/entrada para rotear o áudio do sistema.
  - **Opção B (Gravação):** **OBS Studio** – captura o “WASAPI loopback” (áudio do sistema) e pode gravar ou monitorar.

---

## Opção A — VB-Audio Virtual Cable (rotear áudio do sistema para o Perssua)
Use quando quiser que os apps "enxerguem" o áudio do sistema como se fosse um microfone.

### Passos
1. **Instale o VB-Audio Virtual Cable** e reinicie se solicitado.
2. Abra **Configurações de Som do Windows → Sistema → Som → Saída** e defina **CABLE Input (VB-Audio Virtual Cable)** como **saída padrão** (ou altere apenas o app desejado em *Preferências de volume e dispositivo do app*).
3. Em **Entrada**, confirme que **CABLE Output** existe (é o “microfone” virtual que carrega o áudio do sistema).
4. No **Perssua → Settings → Audio**, escolha **CABLE Output** como **input device** para enviar o áudio do sistema ao app.
5. *(Monitoramento opcional)* Se quiser ouvir o som enquanto roteia:
   - Abra **Painel de Controle → Som → Gravação**.
   - Clique duas vezes em **CABLE Output** → aba **Ouvir** → ative **Ouvir este dispositivo** e escolha seus alto-falantes/headset reais.
6. Reproduza um vídeo ou música de teste e verifique se o medidor de entrada se move no Perssua.

### Observações
- Mantenha o volume moderado para evitar distorção.
- Se só precisar rotear um app (ex: navegador), use **Opções avançadas de som** para selecionar o dispositivo de saída por app, sem mudar o padrão do sistema.

---

## Opção B — OBS Studio (gravação/monitoramento WASAPI Loopback)
Use quando preferir gravar/monitorar o áudio do sistema e, opcionalmente, salvar arquivos.

### Passos
1. Instale o **OBS Studio**.
2. No OBS, clique em **+** em **Sources** → **Audio Output Capture** → escolha **Capture audio** → selecione seu **system output device** (ou **Default**).
3. Alternativamente, use **WASAPI (Loopback)** selecionando o dispositivo de reprodução exato para capturar o áudio do sistema com precisão.
4. Para **monitorar** o que está sendo capturado:  
   - Vá em **Edit → Advanced Audio Properties**.  
   - Para a fonte de saída, defina **Audio Monitoring = Monitor and Output** (escolha seus headphones como Monitoring Device em **Settings → Audio**).
5. Para **gravar**, defina o formato em **Settings → Output** e pressione **Start Recording**.
6. Se quiser enviar isso ao Perssua, combine o OBS com um dispositivo virtual (ex: VB-Cable) e direcione a saída do OBS para a entrada virtual que o Perssua usa.

---

## Verificar no Perssua
1. Abra **Settings → Audio** e selecione a **Input** desejada:
   - **CABLE Output** (Opção A), ou seu microfone normal se só gravar no OBS (Opção B).
2. Fale/reproduza áudio e veja o medidor de entrada.
3. Faça um teste rápido (ex: transcrição ou análise) para confirmar.

---

## Atalhos
- **VB-Audio Virtual Cable:** sem atalhos globais nativos (roteamento é persistente).  
  - *Tip:* If you need quick toggles, consider creating system-wide hotkeys via **AutoHotkey** (optional).
- **OBS Studio:** configure your own hotkeys in **Settings → Hotkeys** (e.g., *Start/Stop Recording*, *Mute/Unmute*, *Toggle Audio Monitoring*).
---

## Tips
- If audio sounds distorted, lower the source app’s volume and/or reduce Windows output level.
- Keep only one “listen/monitor” path active to avoid echo/feedback.
- On laptops with power saving, disable “audio enhancements” and set **High performance** for consistent capture.

## Troubleshooting
- **No signal in Perssua:** Ensure the correct **Input** is selected (e.g., *CABLE Output*) and that the source app is routed to **CABLE Input**.
- **Echo/feedback:** Disable duplicated monitoring (uncheck *Listen to this device* or set OBS monitoring to *Monitor (Off)*).
- **OBS recording silent:** Verify the correct playback device is chosen for **Audio Output Capture** or use **WASAPI Loopback** of the exact device.
- **Choppy audio:** Close heavy apps, lower OBS recording bitrate, or switch power plan to **High performance**.