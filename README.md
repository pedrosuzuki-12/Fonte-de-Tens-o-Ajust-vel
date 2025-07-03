# Fonte de tensão ajustável

*trabalho da disciplina Eletronica para Computação - SSC0180*

# Sobre o projeto
Neste projeto, criamos uma fonte de alimentação capaz de transformar a tensão alternada (AC) da tomada em uma tensão contínua (DC) ajustável, variando de 3V a 12V, com uma corrente máxima de 100mA.

Para desenvolver essa solução, começamos com a fase de simulação, utilizando ferramentas como Falstad e Eagle para testar e refinar o design do circuito. Com o projeto validado, partimos para a construção física da fonte. 

# Tabela dos componentes
| componente | quantidade | custo unitário |
| :----: | :----: | :----: |
|diodo zener|1|R$0,50|
|capacitor 1000uF|1|R$1,50|
|ponte retificadora|R$3,90|
|potenciometro|1|R$7,00|
|resistor 100 (5W)|1|R$1,90|
|resistor 1k|1|R$0,07|
|resistor 4.7k|1|R$0,07|
|transistor|1|R$0,70|
|protoboard|1|R$21,70|
| | **`TOTAL:`** | **`R$37,34`** |

# Sobre os componentes
- **transformador**: reduz a tensão alternada (AC) de 127V, para uma faixa de tensão alternada menor, entre 3V e 12V. Ele é essencial para a segurança e a viabilidade do circuito.
- **ponte retificadora**:  força a corrente a fluir em uma única direção, transformando-a em corrente contínua (DC) pulsante. Ela "endireita" o fluxo da eletricidade, tornando-o adequado para a maioria dos dispositivos eletrônicos.
- **capacitor**: A corrente contínua que sai da ponte de diodos ainda não é perfeitamente estável; ela apresenta "ondas" ou ondulações (ripple). O capacitor atua como um reservatório de energia que filtra essas ondulações. Ele armazena carga quando a tensão está alta e a libera quando a tensão da fonte cai, preenchendo as "lacunas" e suavizando a corrente, aproximando-a de uma linha reta. Isso garante que a energia fornecida seja mais uniforme e confiável, crucial para o bom funcionamento do restante do circuito e do que ele irá alimentar.
- **led**: tem função de indicar o nível da corrente atingida na parte final do circuito. Ele não interfere nos valores obtidos no circuito, servindo como um "feedback" visual de intensidade.
- **diodo zener**: é um componente de segurança e estabilização. Quando a tensão em seus terminais tenta ultrapassar 13V, ele "conduz" a corrente de forma a limitar a tensão nesse valor. Se a tensão for menor que 13V, ele simplesmente não conduz e não interfere. Sua função é proteger o circuito de picos de tensão e garantir que a voltagem nunca exceda um limite seguro para os componentes seguintes, especialmente o potenciômetro e o transistor.
- **potenciômetro**: O potenciômetro é um resistor variável, o que significa que sua resistência pode ser alterada manualmente. No seu circuito, ele é a interface principal para você controlar a tensão de saída, permitindo que você a ajuste de 3V a 12V. Ao girá-lo, você modifica a quantidade de resistência no caminho da corrente, controlando a voltagem que chega aos componentes finais.
- **transistor**: age como uma chave controlada por corrente, mas também como um amplificador. Uma pequena corrente que flui para sua "base" (um de seus terminais) controla uma corrente muito maior que passa entre seus outros terminais. No seu circuito, ele amplifica a corrente que recebe do potenciômetro para um valor desejado, com um máximo de 100mA. Ele é fundamental para fornecer a corrente necessária à carga (o dispositivo que será alimentado pelo seu circuito) e para regular essa corrente de forma eficiente com base no ajuste do potenciômetro.
- **resistores**: limita o fluxo de corrente para proteger outros componentes. Eles também podem atuar como divisores de tensão, ajudando a ajustar níveis de voltagem em partes específicas do circuito.


# Imagem do circuito no Falstad


# PCB no Eagle


# Vídeo do funcionamento e fotos da fonte







# Integrantes

