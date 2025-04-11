# Lines of Action

**Lines of Action** é um jogo de tabuleiro estratégico para dois jogadores implementado em Python usando Pygame. O objetivo é conectar todas as suas peças em um único grupo enquanto impede o adversário de fazer o mesmo. Esta versão suporta modos jogador contra jogador (PvP) e jogador contra inteligência artificial (PvIA), com várias opções de algoritmos de IA.

## Funcionalidades
- **Modos de Jogo**:
  - **PvP**: Dois jogadores humanos competem no mesmo dispositivo.
  - **PvIA**: Jogue contra a IA com diferentes algoritmos e níveis de dificuldade.
- **Algoritmos de IA** (sob "Player vs AI"):
  - **Classic**: Minimax, Alpha-Beta, Negamax, MCTS e Random (movimentos aleatórios).
  - **Heuristic**: Os mesmos algoritmos com uma função de avaliação heurística avançada.
  - Níveis de dificuldade: Easy e Hard (exceto Random).
- **Interface**:
  - Menu interativo com suporte a tela cheia (tecla F) e rolagem.
  - Tabuleiro 8x8 com peças pretas (B) e brancas (W), visualizando movimentos válidos.
- **Regras**:
  - Mova uma peça na horizontal, vertical ou diagonal pelo número exato de peças na linha.
  - Capture peças adversárias pousando sobre elas; conecte todas as suas peças para vencer.

## Requisitos
- Python 3.x
- Pygame (`pip install pygame`)

## Como Executar
1. Clone ou baixe este repositório.
2. Certifique-se de que o Pygame está instalado.
3. Execute o script principal:
   ```bash
   python lines_of_action.py
   ```
   (Substitua `lines_of_action.py` pelo nome do arquivo do código.)

## Uso
- No menu, clique em "PLAYER VS PLAYER" para PvP ou "PLAYER VS AI" para PvIA.
- Em PvIA, escolha entre "Classic" ou "Heuristic", selecione um algoritmo e, se aplicável, um nível de dificuldade.
- Durante o jogo, clique para selecionar e mover peças (apenas movimentos válidos são permitidos).
- Pressione F para alternar entre tela cheia e janela.