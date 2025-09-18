# ♟️ ChessBot Inteligente

Este projeto é um jogo de xadrez aprimorado, com um bot que pensa estrategicamente, um tabuleiro visualmente personalizado e música de abertura. Ideal para quem busca uma experiência de jogo mais envolvente e desafiadora.

---

## 🚀 Funcionalidades Principais

### 🤖 Bot Inteligente
- Algoritmo **Minimax** com **poda alfa-beta** e profundidade 4.
- Avaliação avançada do tabuleiro:
  - Valor das peças (material).
  - Controle do centro (bônus para peças posicionadas no centro).
  - Mobilidade (mais opções de movimento recebem bônus).
  - Penalização para peças que não se moveram (exceto peões).
  - Reconhecimento de situações de **xeque** e **xeque-mate**.

### 🧩 Ajustes Técnicos
- Cada peça possui o campo `type` e o método `getType()`, utilizando o `enum PieceType`.
- Métodos adaptados na classe `Board` para:
  - `isKingInCheck`
  - `isCheckmate`
  - `isGameOver`
- Correção no uso de `getColumn()` (substituindo `getCol()`) e uso do método `isInCenter()` para facilitar a avaliação do controle central.

### 🎨 Personalização Visual
- Casas brancas → verdes  
- Casas pretas → azuis  
- Visual mais agradável e único para o tabuleiro.

### 🎵 Música de Abertura
- Arquivo `inicio.wav` localizado na pasta `resources`.
- Reprodução automática ao iniciar o jogo, utilizando a API `javax.sound.sampled`.

---

## 📁 Estrutura do Projeto
