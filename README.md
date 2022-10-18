# Projeto Predição Diabetes

### Objetivo

Esse projeto teve como objetivo criar um modelo de Machine Learning que consegue prever se um paciente tem diabetes através do estudo e manipulação de um dataset disponível no Kaggle no seguinte link: [https://www.kaggle.com/datasets/akshaydattatraykhare/diabetes-dataset](https://www.kaggle.com/datasets/akshaydattatraykhare/diabetes-dataset)

<div align = 'center'>
 <img src= 'https://user-images.githubusercontent.com/114163919/196523962-d22b6546-a323-4c6a-8a0b-ef775248d733.png' width = '30%'/>
</div>

### Sobre o Dataset

Está disponível no Kaggle, conforme citado anteriormente, porém, foi originalmente disponibilizado pelo *National Institute of Diabetes and Digestive and Kidney Diseases* e possui determinadas medidas de diagnóstico de pacientes do sexo feminino, com idade mínima de 21 anos de herança de um grupo indígena.

As *features disponibilizadas são as seguintes:*

- Pregnancies: expressa o número de gravidez que a pessoa já teve;
- Glucose: expressa a concentração de glicose no sangue;
- BloodPressure: expressa a pressão sanguínea;
- SkinThickness: expressa a espessura da pele;
- Insulin: expressa o nível de insulina no sangue;
- BMI: expressa o índice de massa corporal (IMC);
- DiabetesPedigreeFunction: expressa o percentual da pessoa adquirir diabetes com base em histórico familiar;
- Age: expressa a idade;
- Outcome: expressa se a pessoa tem diabetes ou não (1 para positivo e 0 para negativo).

<div align = 'center'>
 <img src= 'https://user-images.githubusercontent.com/114163919/196524266-087cf3f2-cc06-4b53-b5d4-1c012216f710.png' width = '75%'/>
</div>

### O Projeto

Primeiramente, a base foi importada e visualizada para um entendimento geral. Após isso, realizaram-se as primeiras análises exploratórias e visualização das principais informações estatísticas.

Durante a análise exploratória e visualização das informações estatísticas, surgiu a necessidade da realização de tratamento em algumas colunas/linhas da base, pois algumas apresentavam outliers bem extremos e outras possuem vários valores zerados. Sendo assim, foi preciso realizar o tratamento dessas informações para termos dados dispostos de uma forma melhor.

Com o tratamento feito, 3 modelos de machine learning foram escolhidos para serem utilizados e testados, sendo eles: Perceptron, DecisionTreeClassifier e SVC. Os modelos foram treinados, testados e os resultados foram medidos através da matriz de confusão e de sua acurácia. 

<div align = 'center'>
 <img src= 'https://user-images.githubusercontent.com/114163919/196524541-1396bfa0-612a-40e6-be3f-fb38989b2757.png' width = '30%'/>
</div>

Olhando apenas essas 2 métricas, as seguintes conclusões puderam ser tiradas:

- Falando somente da acurácia, o modelo SVC mostrou-se um pouco melhor que o modelo de DecisionTreee, com acurácias de 78,42% e 73,16% respectivamente.
- O modelo SVC apresenta poucos resultados falsos positivos, porém, apresenta muitos resultados falsos negativos.
- O Perceptron foi o modelo que apresentou menor quantidade de resultados falsos negativos, porém, foi o que mais errou no parâmetro falso positivo.
