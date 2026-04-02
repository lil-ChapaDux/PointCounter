# Dominó — Contador de Pontos

Aplicação web mobile-first para contar pontos em jogos de dominó. Funciona directamente no browser, sem instalação.

## Funcionalidades

* 2 a 4 jogadores com nomes personalizáveis

* Botões rápidos (+5, +10, +15, +20, +25, +30) com design de alto contraste

* Campo de valor personalizado — qualquer múltiplo de 5

* Barra de progresso por jogador em relação à meta definida

* Meta configurável — 100, 200 ou 500 pontos

* Líder destacado com coroa e contorno dourado

* Animação progressiva de contagem ao adicionar pontos

* Desfazer a última jogada

* Histórico completo de todas as rondas com pontuações cumulativas

* Persistência de dados (LocalStorage) — o jogo é guardado e retomado automaticamente

* Classificação Geral (Leaderboard) — regista histórico de vitórias, média de pontos e posições nos últimos 5 jogos

* Reiniciar partida sem sair das configurações

* Wake Lock API — mantém o ecrã ligado durante o jogo (onde suportado)

* Ficheiro HTML único, funciona offline, sem dependências externas

## Como usar

### Abrir directamente

Basta abrir o ficheiro `index.html` num browser. Não é necessário servidor.

### GitHub Pages

1. Faz fork deste repositório

2. Vai a **Settings → Pages**

3. Selecciona o branch `main` como source

4. Acede ao URL gerado

## Como jogar

1. Escolhe o número de jogadores (2–4), define os nomes e a pontuação meta

2. Prime **JOGAR** para iniciar

3. Regista pontos com os botões rápidos ou pelo campo `+outro` (múltiplo de 5)

4. `Desfazer` reverte a última jogada

5. `Histórico` mostra todas as jogadas e pontuações acumuladas por ronda

6. `Reiniciar` repõe todos os pontos a zero

7. `Terminar` conclui a partida, distribui os pontos de vitória e grava na Classificação Geral

8. `Config` volta ao ecrã de configuração

9. No ecrã de configuração, utiliza **🏆 CLASSIFICAÇÃO GERAL** para consultar as estatísticas e ordenar resultados

## Tecnologias

|  |  | 
 | ----- | ----- | 
| HTML5 | Estrutura | 
| CSS3 (Custom Properties, Grid, Flexbox) | Layout e tema escuro | 
| JavaScript (ES5+) | Lógica de jogo e animações | 
| LocalStorage API | Persistência do estado de jogo e classificações | 
| Wake Lock API | Manter ecrã activo | 

## Regras de pontuação

### Pontos de Partida

A aplicação valida que todos os valores inseridos sejam múltiplos de 5, seguindo a regra padrão do dominó.

### Pontos de Classificação Geral

Ao concluir um jogo através do botão `Terminar`, os pontos de vitória são distribuídos pela fórmula: `Pontos = Total de Jogadores - Posição Final`.

| Posição | 2 Jogadores | 3 Jogadores | 4 Jogadores | 
 | ----- | ----- | ----- | ----- | 
| **1º** | 1 | 2 | 3 | 
| **2º** | 0 | 1 | 2 | 
| **3º** | \- | 0 | 1 | 
| **4º** | \- | \- | 0 | 

**Regra de Desempate:** Jogadores com pontuação igual na partida partilham os pontos de vitória relativos à posição mais alta aplicável. O jogador classificado a seguir recebe os pontos relativos à sua posição numérica absoluta na tabela.

## Contribuições

* Claude

* Gemini

## Licença

MIT
