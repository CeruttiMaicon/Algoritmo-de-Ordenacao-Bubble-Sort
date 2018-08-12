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

## Melhorando o Bubble Sort

Agora veremos um pequeno ajuste no algoritmo do Bubble Sort para ajudar ele no seu desempenho com vetores que já vem ordenados. Concordamos que se ele já está ordenado ele não necessita fazer algumas etapas de veritificação, o que faz com que o número de interações seja bem menor. Veja abaixo como a classe BubbleSort2 tem sido utilizada, e como o número de interações mudou.

![
](https://lh3.googleusercontent.com/QHUEoUWY3WK3I3_hCoSzwOjTEV-DX8xKJJofGnnb0WPIUmOuR5WnhXGQLIVtJx5_zGhGWmQtpMWV6A "Vetor ordenado com o BubbleSort2")

Em um vetor crescente o número de interações despencou para 9, assim o número de interações com um vetor de tamanho N é N - 1.

Vejamos aqui como os gráficos se comportam.

![enter image description here](https://lh3.googleusercontent.com/QRCOEosAJuh_l3mphFS0M60Bha6We4SjmtjArhXclld1m-CG687xAHgdsSCHEbf6QRDU1XtYrw_n_w "BubbleSort2")

## Comparação do Algoritmo SelectionSort com o BubbleSort e BubbleSort2

Assim conseguimos concluir que o algortimo BubbleSort 2 tem um desempenho gigantesco pois o número de interações que ele faz com um algoritmo já ordenado é bem pequeno, porem em seu pior caso e no caso médio ele se apresenta ainda pior que o Selection Sort e o BubbleSort1 (da primeira versao do código).

![
](https://lh3.googleusercontent.com/rROl2NDCJgZ2zgqDxLBWjUIcJoW61zh4kiT1IXHPCgpcajdMyu0oa_GlYbzwB0LSonN3h1Zo41Si1A "Grafico de comparação algoritmo bublesort2")



## Sobre o trabalho

Os dados utilizados para gerar o gráfico são do retorno do algoritmo criado neste projeto. O arquivo CSV utilizado para a criação dos gráficos se encontra dentro da pasta "src".

## Execução
No código da Classe MainCSV na linha 15, existe uma tag que deve ser mudada para gerar o arquivo CSV, ali eu especifiquei uma pasta do meu ambiente de trabalho no Ubuntu, mas deve-se trocar o local de criação do arquivo.

Após a execução do algoritmo e receber a mensagem de "Arquivo CSV criado com Sucesso!" o seu arquivo CSV é criado. E com ele eu criei o gráfico da imagem acima.
