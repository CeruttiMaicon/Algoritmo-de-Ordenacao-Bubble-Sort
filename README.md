# Algoritmo de Ordenação Bubble Sort

O algoritmo tem como principal caracteristica manter duas interações de ciclos de repetição. 

Uma executando fixamente com o primeiro valor encontrado enquanto a outra faz uma verificação para fazer a comparação com os outros valores do vetor e durante esse. E durante esse segundo ciclo se o valor inicial for menor do que o valor que esta sendo comparado os valores devem trocar de valor.

## Desempenho do algoritmo

O algoritmo em si se utiliza de seus meios de comparação para ordenar o vetores, mas além das suas linhas de código ele depende muito do tamanho dos arrays recebidos e se eles estao ordenados ou não. No exemplo da imagem abaixo eu utilizei um array com 10 posições, um ordenado de forma Crescente, um Decrescente e um Desordenado (Aleatório). Esses arrays representam o melhor, pior e caso médio que este algoritmo pode apresentar em termos de número de interações necessarias para se fazer a ordenação.

![enter image description here](https://lh3.googleusercontent.com/1DNEL_TqfPWGPMzjGe7C2zNKnBIx4ajQLDDMa5XlOgzh2yZRCtIOz-XiERAZiDzIq4EOC6QKG-DftA "AlgoritmoBubbleSort")

## Testes de desempenho

Agora fazendo os mesmos testes com vetores de 1 a 100, gerados com valores Crescentes, Decrescentes e Aleatorios, fazendo com que o algoritmo escrevece a quantidade de interações feitas com cada tipo de vetor, conseguimos retirar um gráfico no Br Office Calc e obtemos os seguintes resultados apresentados no gráfico a seguir.

![enter image description here](https://lh3.googleusercontent.com/UZvSPw2Kp446bl7Twlp26PtYvpotKrQ7Q0e3jdHp5wQh5dLle7Fdbk2cfJG5sWGVFSyzxyQIOeDmBg "Grafico de Interações do algoritmo Bubble Sort")

## Comparação do Algoritmo SelectionSort com o BubbleSort

Como apresentado no gráfico abaixo temos o numero de interações que cada um dos algoritmos nos trás, estando no pior caso, caso médio ou pior caso, independente do tamanho do array ele sempre cresce de uma forma exponencial. O gráfico mostra de uma forma mais clara o seu número de interações.

![enter image description here](https://lh3.googleusercontent.com/R2mbTKjFrHGQVOzOylpX2gv6nb6qlewgTmz7x2sqOPPF99EO-l59qqf0vKx8coQLdM40R9wtxyuCSA "Gráfico de Interações do algoritmo BubbleSort e SelectionSort")

## Sobre o trabalho

Os dados utilizados para gerar o gráfico são do retorno do algoritmo criado neste projeto. O arquivo CSV utilizado para a criação do gráfico se encontra dentro da pasta "src" com o nome de "arrayBubbleSort.csv".

## Execução
No código da Classe MainCSV na linha 15, existe uma tag que deve ser mudada para gerar o arquivo CSV, ali eu especifiquei uma pasta do meu ambiente de trabalho no Ubuntu, mas deve-se trocar o local de criação do arquivo.

Após a execução do algoritmo e receber a mensagem de "Arquivo CSV criado com Sucesso!" o seu arquivo CSV é criado. E com ele eu criei o gráfico da imagem acima.
