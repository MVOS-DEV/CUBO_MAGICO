Cubos 3D em ASCII

 Este projeto é uma implementação em C que renderiza cubos 3D rotacionando em tempo real diretamente no terminal, utilizando apenas caracteres ASCII.
O código faz uso de cálculos trigonométricos para simular a rotação dos cubos e um buffer de profundidade (z-buffer) para garantir que as superfícies mais próximas sejam desenhadas corretamente.
✨ Funcionalidades

    Renderização de múltiplos cubos em diferentes tamanhos e posições.

    Rotação contínua nos três eixos (A, B, C).

    Uso de diferentes caracteres ASCII para representar cada face dos cubos.

    Compatível com Linux/Unix e Windows (implementação própria de usleep para Windows).

    Animação em tempo real no terminal.

⚙️ Como compilar e executar
Linux / macOS
-bash

gcc cubos.c -o cubos -lm
./cubos

---------------------------------------------

Windows (MinGW)
bash

gcc cubos.c -o cubos -lm
cubos.exe

    ⚠️ Certifique-se de compilar com a flag -lm para linkar a biblioteca matemática.

📂 Estrutura do código

    Transformações 3D: funções calculateX, calculateY, calculateZ aplicam rotação nos eixos.

    Projeção: converte coordenadas 3D para 2D usando perspectiva.

    Z-buffer: garante que apenas a face visível seja desenhada.

    Loop principal: atualiza os ângulos de rotação e redesenha os cubos a cada frame.

🔧 Personalização

Você pode alterar:

    cubeWidth: tamanho dos cubos.

    incrementSpeed: precisão da malha (quanto menor, mais detalhado).

    backgroundASCIICode: caractere usado como fundo.

    K1 e distanceFromCam: parâmetros da projeção.

📜 Licença

Este projeto é de código aberto e pode ser utilizado para fins educacionais, experimentais ou artísticos.
