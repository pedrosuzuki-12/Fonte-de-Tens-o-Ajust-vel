# Fonte de tensão ajustável

*trabalho da disciplina Eletrônica para Computação - SSC0180*

# Sobre o projeto
Neste projeto, criamos uma fonte de alimentação capaz de transformar a tensão alternada (AC) da tomada em uma tensão contínua (DC) ajustável, variando de 3V a 12V, com uma corrente máxima de 100mA.

Para desenvolver essa solução, começamos com a fase de simulação, utilizando ferramentas como Falstad, Tinkercad e Eagle para testar e ajustar o design do circuito para depois fazer o projeto físico em uma protoboard.

# Integrantes

- Pedro Vitor Suzuki Lau - 13837133 
- Gustavo Henrique Brunelli - 11801053
- Christian Bernard - 11795572
- Philippe Sardenberg Castro Couto - 16897421

# Tabela dos componentes
| componente | quantidade | valor total |
| :----: | :----: | :----: |
|diodo zener|1|R$0,50|
|capacitor 1000uF|1|R$1,50|
|ponte retificadora|1|R$3,90|
|potenciômetro|1|R$7,00|
|resistor 100 (5W)|1|R$1,90|
|resistor 1k|10|R$0,70|
|resistor 4.7k|10|R$0,70|
|led|1|R$0,50|
|transistor|1|R$0,70|
|protoboard|1|R$21,70|
| | **`TOTAL:`** | **`R$39,10`** |

# Sobre os componentes
- **transformador**: reduz a corrente alternada (AC) de 127V da tomada, para uma faixa de tensão alternada menor de acordo com a razão entre o número de espiras de um lado para o outro do componente.
- **ponte retificadora**:  força a corrente a fluir em uma única direção, transformando-a em uma corrente contínua (DC) pulsante.
- **capacitor**: A corrente contínua que sai da ponte de diodos apresenta vestígios do corrente alternada, com picos e vales com grande amplitude. Ela apresenta "ondas" ou ondulações (ripple). O capacitor atua como um reservatório de energia que filtra essas ondulações. Ele armazena carga quando a tensão está alta e a libera quando a tensão cai, preenchendo as "lacunas" e suavizando a corrente, aproximando-a de uma linha reta.
- **led**: tem função de indicar a passagem da corrente atingida na parte do meio do circuito. Ele não interfere resto obtidos do circuito, servindo apenas como um "feedback" visual.
- **diodo zener**: é um componente de segurança e estabilização. Quando a tensão em seus terminais tenta ultrapassar 13V, ele "conduz" a corrente de forma a limitar a tensão nesse valor. Se a tensão for menor que 13V, ele funcionz como um fio. Sua função é proteger o circuito de picos de tensão e garantir que a voltagem nunca exceda um limite seguro para os componentes seguintes.
- **potenciômetro**: O potenciômetro é um resistor variável, o que significa que sua resistência pode ser alterada manualmente. No circuito, ele é a interface principal para controlar a tensão de saída, permitindo ela seja ajustada de 3V a 12V.
- **transistor**: age como uma chave controlada por corrente, mas também como um amplificador. Uma pequena corrente que flui para sua base controla uma corrente muito maior que passa entre seus outros terminais. No circuito, ele amplifica a corrente que recebe do potenciômetro para um valor desejado, com um máximo de 100mA.
- **resistores**: limitam o fluxo de corrente para proteger outros componentes, possibilitando o "controle" da tensão e, por consequência, da corrente e da potência associadas a um componente do circuito.


# Imagem do circuito no Falstad
https://tinyurl.com/2yqzh566

![image](https://github.com/user-attachments/assets/3374c135-d6df-4a32-83b3-f3f7110b05c7)


# PCB no Eagle
![{5D3AD645-4C68-47A2-94C1-5521AD20DE3D}](https://github.com/user-attachments/assets/c422582b-90c5-40c2-bf61-515667d520b0)


![{19CC4951-48AF-44A3-9447-AF82FA42B180}](https://github.com/user-attachments/assets/c6e3d7ae-8a41-4e7f-9b65-25f16a7c0c46)


# Vídeo do funcionamento e fotos da fonte








