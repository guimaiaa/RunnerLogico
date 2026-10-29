# Runner Lógico

Jogo de corrida infinita no navegador para praticar **portas lógicas**. Você é um sinal carregando um bit (0 ou 1) por um circuito de 3 trilhos. Cada trilho tem uma porta lógica com uma entrada fixa: escolha o trilho e o bit certos para que a saída seja **1** e você continue correndo.

Portas: AND, OR, NOT, XOR, NAND, NOR e XNOR, além de bloqueios ✕ (trilhos sem saída).

## Como jogar

Abra o `index.html` em qualquer navegador. Não precisa instalar nada.

| Ação | Teclado | Celular |
|---|---|---|
| Trocar o bit | `Espaço` / clique | Tocar |
| Mudar de trilho | `↑` `↓` ou `W` `S` | Deslizar ↑ ↓ |
| Acelerar / frear | Segurar `→` / `←` ou `D` / `A` | Arrastar → / ← e segurar |
| Pausar | `P` | Botão ⏸ |
| Som | `M` | Botão 🔊 |

**Regra:** saída = PORTA(seu bit, entrada). Saída 1 → passa. Saída 0 → game over.

## Tecnologia

Um único arquivo HTML com CSS e JavaScript puro (Canvas), sem dependências.
