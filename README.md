# Documentação do código

# Tutorial: Quebra-cabeça com números (HTML/JS)

Este projeto implementa um pequeno jogo de lógica apresentado dentro de uma tabela. O usuário pode iniciar preenchendo a tabela com incógnitas (indicadas por "?") e jogar interagindo com as células da tabela para fazer substituições.

## Visão geral
- Gera uma grade (tabela) com 10 linhas e 13 colunas.
- As células contêm números, operadores e símbolos, com algumas posições marcadas por `?` para representar incógnitas.
- Ao clicar em uma célula:
  - Primeiro clique seleciona a célula (com destaque).
  - Segundo clique copia o conteúdo da segunda célula para a primeira.
- Um botão "Reload" recarrega a página, gerando uma nova grade.

## Estrutura do conteúdo (alto nível)

- HTML:
  - Estrutura básica com `<table id="minha-tabela">` para a grade.
  - Um botão que recarrega a página.

- CSS:
  - Aparência da grade: tamanho, cores, bordas, hover, etc.

- JavaScript:
  - Constantes de sinais/operadores.
  - Geração da matriz `matrix` (10x13) com padrões de conteúdo.
  - Inserção de 5 `?` em posições aleatórias por linha.
  - Construção da tabela no DOM a partir da matriz.
  - Lógica de clique em células para selecionar/copiar conteúdo entre células.

## Como o código “joga” (regras de jogo)

- A grade contém números, operadores e símbolos, formando expressões incompletas.

- As incógnitas `?` podem ser trocadas por valores durante o jogo, permitindo ao jogador completar as expressões.
