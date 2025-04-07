
# Lines of Action - linesofaction.py

## Descrição

Implementação do jogo "Lines of Action" (LoA) em Python com Pygame. Inclui modos **Player vs Player (PvP)** e **Player vs IA (PvAI)** com três dificuldades: Fácil (profundidade 1), Difícil (profundidade 3) e Muito Difícil (profundidade 8). A IA usa Minimax com poda alfa-beta. O objetivo é conectar todas as tuas peças num grupo contínuo.

## Funcionalidades

- **Modos**: PvP e PvAI (Fácil, Difícil, Muito Difícil).
- **Interface**: Menu, tabuleiro 8x8, peças pretas/brancas, destaque de movimentos (verde/azul), mensagens de vitória.
- **Regras**: Peças movem-se em linha reta uma distância igual ao número de peças na linha; não podem saltar adversárias, mas podem capturá-las. Vence quem conectar todas as suas peças.

## Requisitos

- **Sistema**: Windows, macOS ou Linux.
- **Python**: 3.6+.
- **Biblioteca**: Pygame (`pip install pygame`).

## Instalação

1. Instala o Python: [python.org](https://www.python.org/downloads/).
2. Instala o Pygame:
   ```bash
   pip install pygame
   ```
3. Descarrega o ficheiro `linesofaction.py`.

## Como Utilizar

1. Executa:
   ```bash
   cd caminho/para/a/pasta
   python linesofaction.py
   ```
2. **Menu**: Escolhe entre "PLAYER VS PLAYER", "PLAYER VS IA (EASY)", "HARD" ou "VERY HARD".
3. **Jogar**:
   - PvP: Alterna entre Preto ("B") e Branco ("W"). Clica para selecionar (verde) e mover (azul).
   - PvAI: Joga como Preto; a IA (Branco) responde automaticamente.
   - O jogo termina ao conectar todas as peças de um jogador.
4. **Sair**: Fecha a janela ou usa `Ctrl+C`.

## Estrutura do Código

- **Imports/Constantes**: Configurações de cores, tamanhos, IA.
- **Menu**: `draw_gradient_background`, `draw_button`.
- **Jogo**: `init_board`, `draw_board`, `is_valid_move`, `compute_valid_moves`, `check_connected`.
- **IA**: `get_ai_move`, `minimax`, `evaluate_board`.
- **Principal**: `iniciar_jogo`, `menu_principal`.

## Problemas Conhecidos

- **Modo Muito Difícil**: Pode ser lento (profundidade 8).
- **Avaliação da IA**: Simples, pode não ser sempre ótima.
