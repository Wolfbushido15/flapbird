
# Flappy Bird Clone - Pygame

Este projeto é uma recriação simples do clássico jogo **Flappy Bird** usando a biblioteca Pygame. O objetivo do jogo é controlar um pássaro e evitar colidir com os canos ou com o chão, obtendo o maior número possível de pontos.

## Funcionalidades

- Controle o pássaro com a tecla `espaço` para fazer ele "bater as asas" e subir.
- O jogo gera automaticamente canos de alturas aleatórias, tanto na parte superior quanto na inferior da tela.
- O chão se move para criar uma sensação de progresso no jogo.
- O jogo termina quando o pássaro colide com um cano ou com o chão.

## Instalação

1. **Clone o repositório**:
    ```bash
    git clone https://github.com/seuusuario/flappy-bird-clone.git
    ```

2. **Instale as dependências**:
    Certifique-se de ter o Pygame instalado:
    ```bash
    pip install pygame
    ```

3. **Adicione os arquivos de imagem**:
    O código faz uso de algumas imagens, certifique-se de ter os seguintes arquivos na mesma pasta do código:
    - `bluebird-upflap.png`
    - `bluebird-midflap.png`
    - `bluebird-downflap.png`
    - `pipe-red.png`
    - `base.png`
    - `background-day.png`

4. **Execute o jogo**:
    Após configurar o ambiente, execute o jogo com o seguinte comando:
    ```bash
    python game.py
    ```

## Como Jogar

- Pressione a tecla **espaço** para fazer o pássaro subir.
- O pássaro será afetado pela gravidade e irá cair automaticamente, então controle bem seus movimentos.
- Evite colidir com os canos e com o chão.

## Estrutura do Código

- **Bird**: Classe responsável por representar o pássaro. Gerencia a animação e a física do voo.
- **Pipe**: Classe que gera os canos (inferiores e superiores) com base em posições aleatórias.
- **Ground**: Classe que gerencia o chão, incluindo a movimentação contínua.
- **Funções auxiliares**:
    - `is_off_screen(sprite)`: Verifica se um objeto (cano ou chão) saiu da tela para removê-lo.
    - `get_random_pipes(xpos)`: Gera um par de canos (um invertido e outro normal) em uma posição aleatória.

## Melhorias Futuras

- Adicionar um contador de pontos.
- Incluir uma tela inicial com um botão para iniciar o jogo.
- Implementar um sistema de dificuldade crescente.
- Criar uma tela de "Game Over" com a opção de reiniciar o jogo.

## Licença

Este projeto é open-source e está licenciado sob a [MIT License](LICENSE).
