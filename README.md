# RobotPascalMaze
Program robo_busca


Introdução
Este trabalho tem como objetivo criar um algoritmo que possibilite implementar uma busca em profundidade interativa. Busquei na internet as aplicações para este tipo de busca e optei por utilizar em “Solução de Labirintos”.

Linguagem e conceito
Utilizei a linguagem pascal por ser mais didática e fácil. Utilizei também princípios do case do robô que limpa quadrados em uma sala.

Construção
Na criação do labirinto delimitei por uma matriz posições possíveis e impossíveis para o robô, assim ele nunca estaria em uma posição que fosse parede ou fora do range do labirinto.
Declarei variáveis de inicio e fim(aleatório) e um estado inicial onde o robô não teria ainda passado por nenhum lugar e inicia sua busca na parte superior esquerda da tela. 
Para que o robô andasse criei ifs dentro de ifs onde a prioridade sempre seria ir para a esquerda. Consiste em ir sempre para o lugar onde tivesse passado menos vezes e em caso de empate optar pela esquerda. 
No exemplo abaixo pode-se ver que o robô sempre irá para baixo:

<img src="/TiagoHucs/RobotPascalMaze/blob/master/imgs/img1.PNG?raw=true" alt="img1.PNG">

9	9	9
9	1	9
9	1	9
9	R	9
9	0	9
9	0	9
 
Da mesma forma em que podemos ver que o robô optará em ir ainda não foi ou onde esteve menos vezes que no exemplo abaixo escolherá ir para a direita:
9	1	9
9	R	0
9	2	9
 
 
No código é possível contar quantos passos o robô andou pois a cada decisão de direção tomada soma-se +1 a um contador. Também defini no meu código que todo ponto sem saída ou intercessão entre caminhos é um só, sendo possível contar quantos nós visitei e quantas vezes visitei cada nó.
A interatividade foi implementada na aleatoriedade do ponto final no labirindo podendo ser uma busca profunda ou raza. Também poderia delimitar  a quantidade de passos ou um limite de nós. Mas não coloquei neste código.

O resultado pode ser visto na imagem abaixo em 2 execuções diferentes do programa:
    
