# Fonte de tensão ajustável

*trabalho da disciplina Eletronica para Computação - SSC0180*

# Sobre o projeto
Nesse trabalho, tivemos a tarefa de criar uma fonte que, recebendo tensão de uma tomada com corrente alternada, tenha capacidade de ajustar a ddp para uma faixa de 3V a 12V e tornar a corrente contínua, que possa atingir o valor de 100mA. Assim, usamos simuladores como o Falstad e o Eagle para elaborar a ideia e, posteriormente, construímos a fonte, cujos detalhes podem ser vistos no decorrer dessa página.

# Tabela dos componentes
| componente | quantidade | custo unitário |
| :----: | :----: | :----: |
|diodo zener|1|R$0,50|
|capacitor 470uF|1|R$4,40|
|ponte retificadora|R$0,20|
|potenciometro|1|R$7,00|
|resistor 100 (5W)|1|R$1,90|
|resistor 1k|1|R$0,07|
|resistor 4.7k|1|R$0,07|
|transistor|1|R$0,80|
|protoboard|1|R$21,70|
| | **`TOTAL:`** | **`R$37,31`** |

# Sobre os componentes
- **transformador**: tem o papel de diminuir a voltagem que o circuito recebe da fonte corrente alternada (tomada). a partir da voltagem de 127V recebida, o transformador consegue diminuí-la para a faixa de tensão desejada (3V a 12V).
- **ponte de diodo**: também chamada de ponte retificadora, é uma junção de 4 diodos que têm a capacidade de transformar a tensão alternada (vinda da tomada) em contínua, ou seja, tem capacidade de a "retificar".
- **capacitor**: armazena carga no circuito nos ciclos da corrente alternada, liberando corrente quando a tensão da fonte é menor do que a tensão interna. ele descarrega sua carga armazenada quando há a inversão do ciclo no circuito. com base em cálculos de um ripple de 10%, chegamos próximos do valor comercial de 470uF de capacitância, usando um capacitor com esse valor no projeto.
- **diodo zener**: tem o intuito de regular a corrente máxima, sendo o usado especificamente de voltagem máxima de 13V. quando a ddp passa de 13V, ele mantém o valor máximo de 13 em seus terminais; quando a ddp chega menor do que 13V, ele não conduz e consequentemente não interfere no circuito.
- **potenciômetro**: é um resistor variável usado como controle da tensão resultante, que permite atingir as ddps de 3V a 12V no circuito.
- **transistor**: amplifica a corrente que recebe em sua base para um valor desejado, sendo o máximo de 100mA.
- **resistores**: usados em mais de um momento no circuito, têm a função de limitar a corrente, garantindo certa "segurança" aos componentes. no circuito, usamos eles associados ao led, ao zener, ao potenciômetro e ao transistor, com resistências variadas de 100, 120, 2.2k e 3k de ohms.
- **led**: tem função de indicar o nível da corrente atingida na parte final do circuito, brilhando mais quando a voltagem e a corrente são maiores. de modo geral, não interfere nos valores obtidos no circuito, servindo unicamente como indicação da voltagem e corrente ajustáveis.

# Imagem do circuito no Falstad


# PCB no Eagle


# Vídeo do funcionamento e fotos da fonte







# Integrantes

