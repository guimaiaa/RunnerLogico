# Runner Lógico

Jogo de corrida infinita no navegador para praticar **portas lógicas**.

🎮 **Jogar:** https://guimaiaa.github.io/RunnerLogico/

## História

Um vírus chamado **Ruído** invadiu o computador e a CPU está se apagando. Você é o **Bit**, o último sinal limpo do sistema: atravesse os **5 setores** do circuito (Barramento de Entrada → Memória RAM → ULA → Cache → Núcleo da CPU) passando pelos portões lógicos e entregue o sinal de reinicialização à CPU. São 40 portões até a vitória; depois o jogo segue no **modo infinito** para bater recorde.

## Como jogar

Você carrega um bit (0 ou 1) por um circuito de 3 trilhos. Cada trilho tem uma porta lógica com uma entrada fixa: escolha o trilho e o bit certos para que a saída seja **1** e continue correndo.

Portas, liberadas uma por setor: NOT, AND, OR → XOR → NAND, NOR → XNOR → IMPLICA (x → e), além dos bloqueios ✕ (trilhos sem saída).

| Ação | Teclado | Celular |
|---|---|---|
| Trocar o bit | `Espaço` / clique | Tocar |
| Mudar de trilho | `↑` `↓` ou `W` `S` | Deslizar ↑ ↓ |
| Acelerar / frear | Segurar `→` / `←` ou `D` / `A` | Arrastar → / ← e segurar |
| Dicas nos portões | `H` | Botão 💡 |
| Pausar | `P` ou `Esc` | Botão ⏸ |
| Som | `M` | Botão 🔊 |

**Regra:** saída = PORTA(seu bit, entrada). Saída 1 → passa. Saída 0 → o Ruído pega o Bit.

## Recursos de aprendizagem

- **Treino guiado** (7 passos): ensina a trocar o bit, mudar de trilho, AND, NOT, bloqueios e velocidade. No treino ninguém perde: se errar, o jogo explica o cálculo e repete o passo.
- **Modo dica 💡**: mostra embaixo de cada portão qual bit passa.
- **Game Over educativo**: mostra o cálculo que deu 0 (ex.: `XOR(1, 1) = 0`) e a tabela-verdade com a linha do erro destacada.
- **Como funcionam as portas**: tabelas-verdade de todas as portas, disponível no menu, na pausa e no Game Over.

## Testes com usuários (AV3)

- **⭐ Avaliar o jogo** (no Game Over): 3 notas de 1 a 5 (diversão, clareza das instruções, aprendizado) e um comentário.
- **📊 Resultados dos testes** (no menu): partidas, treinos, vitórias, taxa de acerto, portões com mais erros e médias das avaliações. Os dados ficam salvos no aparelho, então um computador usado na feira acumula os resultados de todos os jogadores. O botão **Copiar dados (CSV)** exporta tudo para uma planilha.

## Tecnologia

Um único arquivo HTML com CSS e JavaScript puro (Canvas e Web Audio), sem dependências. Ao abrir a página, um teste automático confere as tabelas-verdade e o gerador de portões (resultado no console, F12).
