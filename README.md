# Dominó — Contador de Pontos

Aplicação web mobile-first para contar pontos em jogos de dominó. Funciona directamente no browser, sem instalação.

---

## Funcionalidades

- 2 a 4 jogadores com nomes personalizáveis
- Botões rápidos (+5, +10, +15, +20, +25, +30) para registo ágil de pontos
- Campo de valor personalizado — qualquer múltiplo de 5
- Barra de progresso por jogador em relação à meta definida
- Meta configurável — 100, 200 ou 500 pontos
- Líder destacado com coroa e contorno dourado
- Desfazer a última jogada
- Histórico completo de todas as rondas com pontuações cumulativas
- Reiniciar partida sem sair das configurações
- Wake Lock API — mantém o ecrã ligado durante o jogo (onde suportado)
- Ficheiro HTML único, funciona offline, sem dependências externas

---

## Como usar

### Abrir directamente
Basta abrir o ficheiro `index.html` num browser. Não é necessário servidor.

### GitHub Pages
1. Faz fork deste repositório
2. Vai a **Settings → Pages**
3. Selecciona o branch `main` como source
4. Acede ao URL gerado

---

## Como jogar

1. Escolhe o número de jogadores (2–4), define os nomes e a pontuação meta
2. Prime **JOGAR** para iniciar
3. Regista pontos com os botões rápidos ou pelo campo `+outro` (múltiplo de 5)
4. `Desfazer` reverte a última jogada
5. `Histórico` mostra todas as jogadas e pontuações acumuladas por ronda
6. `Reiniciar` repõe todos os pontos a zero
7. `Config` volta ao ecrã de configuração

---

## Tecnologias

| | |
|---|---|
| HTML5 | Estrutura |
| CSS3 (Custom Properties, Grid, Flexbox) | Layout e tema escuro |
| JavaScript (ES5+) | Lógica de jogo |
| Wake Lock API | Manter ecrã activo |

---

## Regras de pontuação

A aplicação valida que todos os valores inseridos sejam múltiplos de 5, seguindo a regra padrão do dominó.

---

## Contribuições

- Claude

---

## Licença

MIT
