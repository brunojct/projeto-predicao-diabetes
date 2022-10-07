# Projeto Predição Diabetes

### Objetivo

Esse projeto teve como objetivo criar um modelo de Machine Learning que consegue prever se um paciente tem diabetes através do estudo e manipulação de um dataset disponível no Kaggle no seguinte link: [https://www.kaggle.com/datasets/akshaydattatraykhare/diabetes-dataset](https://www.kaggle.com/datasets/akshaydattatraykhare/diabetes-dataset)

<div align = 'center'>
 <img src= 'https://s3.us-west-2.amazonaws.com/secure.notion-static.com/960575dc-4fa4-4d17-ad1b-85fc6f4e0472/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20221007%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20221007T130408Z&X-Amz-Expires=86400&X-Amz-Signature=75a92d82d1dec4a98e8d85620c8e988f783f34829a4634314096b02f44097dbf&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject' width = '30%'>
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
 <img src= 'https://s3.us-west-2.amazonaws.com/secure.notion-static.com/af420c09-0b66-485b-a780-b34c0efe7e32/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20221007%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20221007T130644Z&X-Amz-Expires=86400&X-Amz-Signature=b42c6c5163a08e6e7caeddfa194e89f0c3d830799e29a4fcd6bc28d8996e384d&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject' width = '75%'>
</div>

### O Projeto

Primeiramente, a base foi importada e visualizada para um entendimento geral. Após isso, realizaram-se as primeiras análises exploratórias e visualização das principais informações estatísticas.

Durante a análise exploratória e visualização das informações estatísticas, surgiu a necessidade da realização de tratamento em algumas colunas/linhas da base, pois algumas apresentavam outliers bem extremos e outras possuem vários valores zerados. Sendo assim, foi preciso realizar o tratamento dessas informações para termos dados dispostos de uma forma melhor.

Com o tratamento feito, 3 modelos de machine learning foram escolhidos para serem utilizados e testados, sendo eles: Perceptron, DecisionTreeClassifier e SVC. Os modelos foram treinados, testados e os resultados foram medidos através da matriz de confusão e de sua acurácia. 

<div align = 'center'>
 <img src= 'https://s3.us-west-2.amazonaws.com/secure.notion-static.com/88d1ba25-2066-419e-9b6c-a7ce83161617/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20221007%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20221007T130741Z&X-Amz-Expires=86400&X-Amz-Signature=2fa53e3e2333dbeba0e04a20b97fdac4b47394f14a412a23daa057e9421e9c66&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject' width = '30%'>
</div>

Olhando apenas essas 2 métricas, as seguintes conclusões puderam ser tiradas:

- Falando somente da acurácia, o modelo SVC mostrou-se um pouco melhor que o modelo de DecisionTreee, com acurácias de 78,42% e 73,16% respectivamente.
- O modelo SVC apresenta poucos resultados falsos positivos, porém, apresenta muitos resultados falsos negativos.
- O Perceptron foi o modelo que apresentou menor quantidade de resultados falsos negativos, porém, foi o que mais errou no parâmetro falso positivo.
