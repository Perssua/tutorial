# Prompts & Custom Prompts (Premium)

## Visão Geral
Um **prompt** é o conjunto de instruções que guia a IA sobre *o que fazer*, *como responder* e *em qual contexto*. Prompts bem elaborados geram respostas mais úteis, consistentes e orientadas a objetivos.  
Com o recurso **Custom Prompt (Premium)**, você pode criar templates reutilizáveis para padronizar análise, tom de voz e foco entre equipes e projetos.

## Por que prompts são importantes
- **Clareza → melhor resultado:** instruções claras reduzem ambiguidades.  
- **Contexto certo:** os resultados são mais relevantes quando a IA sabe *para quem* e *por quê*.  
- **Consistência entre usuários:** templates ajudam diferentes pessoas a manter o mesmo padrão de qualidade.  
- **Velocidade:** menos retrabalho e menos pedidos de ajuste.

### Blueprint de prompt (recomendado)
Inclua estes blocos no seu template:
- **Role:** “Você é um analista pré-vendas focado em contornar objeções.”  
- **Objective:** “Resuma a call em 5 tópicos com próximos passos.”  
- **Context:** público, produto, restrições, exemplos.  
- **Style & Constraints:** tom, formato (Markdown/tabela), limites de palavras ou tokens.  
- **Inputs:** variáveis como `{client}`, `{product}`, `{language}`, `{goal}`.

## Pré-requisitos
- Plano Perssua ativo.  
- Permissão para salvar configurações (Custom Prompt requer **Premium**).  
- (Opcional) Fontes de input: transcrições, screenshots, anotações.

---

## Passos — Usando um prompt padrão
1. Abra **Features → Prompts**.  
2. Selecione um **Prompt** da lista (ex: *Call Summary*, *Objection Analysis*).  
3. (Opcional) Preencha variáveis (ex: `{language = en-US}`).  
4. Clique em **Apply** e envie seu input (texto/áudio/screenshot) pelo chat.  

## Passos — Criando um Custom Prompt (Premium)
1. Vá em **Settings → Prompts → New Custom Prompt**.  
2. Adicione um **Name** e **Description**.  
3. Cole o conteúdo do seu template (use o *blueprint* acima).  
4. Adicione **Variables** (ex: `{client}`, `{goal}`, `{language}`) e defina valores padrão.  
5. (Opcional) Marque **Set as default** para:  
   - Um recurso específico (ex: Whisper / Screenshot Analysis).  
   - Um contexto (ex: *Demos*, *Support*, *Onboarding*).  
6. Salve com **Create**.  
7. No chat, selecione seu **Custom Prompt** e **Apply** antes de enviar o input.  

## Configurações de Áudio (para prompts usados com Whisper)
- **Input device:** escolha o microfone correto em **Settings → Audio**.  
- **Input level & noise suppression:** ajuste para evitar distorção ou ruído de fundo.  
- **Language:** defina seu idioma principal para melhor transcrição.  

---

## Atalhos
> *Não há atalho global padrão para abrir Prompts.*  
> Se disponível, vá em **Settings → Shortcuts** para criar um atalho para “Open Prompts.”  

Atalhos úteis relacionados:  
- **Ctrl + D** — Gravar & transcrever áudio (Whisper).  
- **Ctrl + E** — Capturar screenshot.  
- **Ctrl + Enter** — Analisar o screenshot mais recente.  
- **Ctrl + Up/Down** — Rolar o chat do Perssua.  
