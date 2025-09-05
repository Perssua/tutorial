# Captura de Screenshot & ASK Context

## Visão Geral
Use screenshots para mostrar à IA exatamente o que você vê na tela e pedir uma análise direcionada. Você pode capturar uma ou várias screenshots, adicionar um **ASK** (instrução ou pergunta que dá contexto extra) e então enviar tudo para análise.

## Pré-requisitos
- Permissões de captura de tela concedidas pelo sistema (Windows/macOS).
- Perssua aberto e ativo.
- Conexão de internet estável.

---

## Passos

### A) Capturar screenshots
1. Abra a página/app que deseja analisar.
2. Pressione **Ctrl + E** para capturar um screenshot.  
   - Repita **Ctrl + E** para adicionar mais screenshots ao mesmo pedido (lote).
3. (Opcional) Remova capturas indesejadas da fila (Trash/Remove na miniatura).

### B) Adicionar contexto com **ASK**
4. No campo **ASK**, digite uma instrução ou pergunta concisa para guiar o modelo.  
   - Exemplos:  
     - “Encontre problemas de UI e sugira correções.”  
     - “Resuma os principais erros do console e próximos passos.”  
     - “Onde está o botão de preços nesta página?”  
   - Seja específico e objetivo.

### C) Analisar
5. Pressione **Ctrl + Enter** para analisar as screenshots capturadas **ou** clique em **Analyze**.
6. Revise a resposta do modelo no chat.
7. Se necessário, itere: capture outro screenshot (**Ctrl + E**) e refine o **ASK**.

---

## Limites do plano gratuito
- **Screenshots por análise (Free):** até **X** screenshots por pedido.  
  > Substitua **X** pelo limite atual do seu plano gratuito (ex: **3**). Veja **Settings → Plan** para os limites mais recentes.  
- Lotes maiores e histórico ampliado estão disponíveis em planos pagos.

---

## Atalhos
- **Ctrl + E** — Capturar screenshot.  
- **Ctrl + Enter** — Analisar as screenshots mais recentes.  
- **Ctrl + Up/Down** — Rolar o chat do Perssua para cima/baixo. 

---

## Dicas
- **Seja específico no ASK:** “Destaque espaçamentos inconsistentes e proponha correções em CSS” é melhor que “Melhorar design”.
- **Agrupe de forma inteligente:** Junte telas relacionadas (ex: Página → Modal → Estado de erro) em um pedido para manter o contexto.
- **Oculte dados sensíveis** antes de capturar ou use blur na região se necessário.
- **Ciclos rápidos:** **Ctrl + E** → **Ctrl + Enter** acelera o processo de iteração.

## Solução de Problemas
- **Atalho não funciona:** Verifique se o Perssua está em foco ou se outro app está interceptando o atalho.
- **Imagens em branco/preto no macOS:** Reative a permissão de **Screen Recording** para o Perssua e reinicie o app.
- **Falha no upload:** Verifique a conexão; capturas grandes ou de alta resolução podem demorar — tente uma região menor.
- **Respostas irrelevantes:** Refine o **ASK** com intenção mais clara (o que checar, restrições, formato desejado).
