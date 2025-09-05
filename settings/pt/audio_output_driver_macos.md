
# Captura de Áudio de Saída no macOS (Terceiros)

## Visão Geral
Por padrão, o macOS **não** permite que apps capturem diretamente o áudio do sistema/saída (“o que você ouve”).  
Para permitir que o Perssua analise ou transcreva sons do sistema (ex: chamadas, músicas, vídeos), é necessário um app de terceiros que crie um **dispositivo de áudio virtual**. Ele atua como um canal intermediário entre a saída do Mac e o Perssua.

---

## Pré-requisitos
- macOS 12 ou superior.
- Direitos de administrador no Mac.
- Um dos seguintes apps de terceiros instalado:
	- **BlackHole (gratuito)** — driver de áudio virtual: <https://existential.audio/blackhole/>
	- **Loopback (pago)** — roteamento avançado com interface: <https://rogueamoeba.com/loopback/>
- Perssua instalado e em execução.

---

## Passos — BlackHole (opção gratuita)

### Instalar o BlackHole
1. Baixe o BlackHole do [site oficial](https://existential.audio/blackhole/).
2. Instale o pacote (requer senha de administrador).
3. Reinicie o Mac se solicitado.

### Criar um Multi-Output Device
1. Abra o **Audio MIDI Setup** (busque pelo Spotlight).
2. Clique no botão **+** → **Create Multi-Output Device**.
3. Selecione tanto os **MacBook Speakers** (ou sua saída principal) quanto o **BlackHole**.
4. Clique com o botão direito e escolha **Use This Device for Sound Output**.

### Roteando áudio para o Perssua
1. Em **System Settings → Sound → Output**, selecione o novo **Multi-Output Device**.
	 - Você ouvirá o som pelos alto-falantes/fones, enquanto uma cópia vai para o BlackHole.
2. No **Perssua → Settings → Audio**, escolha **BlackHole** como **input device**.
3. Reproduza um vídeo/música e teste a transcrição ou análise.

---

## Passos — Loopback (opção paga, mais fácil)
1. Instale o **Loopback** da [Rogue Amoeba](https://rogueamoeba.com/loopback/).
2. Abra o Loopback e crie um **New Virtual Device**.
3. Adicione sua saída do sistema (ex: MacBook Speakers) como **Source**.
4. Direcione para um dispositivo **Pass-Thru** para duplicar o áudio.
5. Em **System Settings → Sound → Output**, selecione seus alto-falantes/fones normais.
6. No **Perssua → Settings → Audio**, selecione o dispositivo virtual do Loopback como **input**.

---

## Atalhos
Depois de configurado, use os atalhos do Perssua normalmente:
- **Ctrl + D** — Gravar & transcrever áudio (via BlackHole/Loopback).
- **Ctrl + E** — Capturar screenshot.
- **Ctrl + Enter** — Analisar o screenshot mais recente.
- **Ctrl + B** — Alternar visibilidade do app.

---

## Dicas
- **BlackHole:** Gratuito e leve, mas exige configuração no Audio MIDI Setup.
