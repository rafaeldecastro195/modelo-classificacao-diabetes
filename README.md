# Aplicação web para Pré-Diagnóstico de Diabetes usando Aprendizado Supervisionado

Seja bem-vindo(a) ao repositório!

Projeto de `portfólio` em **estágio de desenvolvimento**.

Em breve será totalmente enviado ao GitHub.

## Sobre o projeto

Trata-se de o desenvolvimento de uma aplicação web, que usa um algoritmo de `Machine Learning` e `Aprendizado Supervisionado de Classificação`, para trazer ao usuário a probabilidade de ele ter o diagnóstico positivo de `diabetes mellitus`, expresso por percentual. A aplicação irá fornecer conselhos e conteúdo sobre o que fazer, de acordo com o percentual de positividade do paciente no contexto. Será assim, pois ***o diagnóstico é feito pelos profissionais de saúde competentes.*** O objetivo é, portanto, incentivar o paciente a buscar ajuda profissional, uma vez que a `diabetes mellitus` possa ter sintomas imperceptíveis.

Nele, é usado o dataset [Diabetes prediction dataset](https://www.kaggle.com/datasets/iammustafatz/diabetes-prediction-dataset/data), disponível na plataforma Kaggle.

Serão testados diferentes Modelos de Classificação para se determinar qual o mais eficiente para o contexto.

## Tecnologias utilizadas

| Tecnologia | Descrição | Onde foi/será utilizado |
| :---: | :---: | :---: |
| `Python` | Linguagem de programação multiuso | Linguagem usada em todo o processo, desde as análises descritivas e preditivas até a aplicação web |
| `Pandas` | Biblioteca de manipulação de dados | Usada em todo o processo de análise de dados, da Análise Exploratória de Dados à criação e teste dos modelos |
| `Numpy` | Biblioteca de cálculo científico | Usada principalmente na Análise Exploratória de Dados, junto ao Pandas |
| `SciPy` | Bibloteca de cálculo científico | Usada para calcular a `Curva Normal Gaussiana` nos histogramas de Matplotlib e Seaborn |
| `Matplotlib` | Biblioteca de visualização de dados | Usada em histogramas e boxplots da Análise Exploratória de Dados, junto a Seaborn |
| `Seaborn` | Biblioteca de visualização de dados | Usada em histogramas e boxplots da Análise Exploratória de Dados, junto a Matplotlib |
| `Scikit-Learn` | Biblioteca para treinamento e testes de modelos de Machine Learning | Separação dos dados em treino e teste, criação de modelos como Logistic Regression |
| `XGBoost` | Biblioteca de otimização de gradiente, baseada em Árvores de Decisão | Criação do modelo, instância de XGBClassifier, que usa o método `.predict_proba()` para calcular a probabilidade |
| `Imbalanced Learn` | Biblioteca para balanceamento de classes | Balanceamento das classes `0` e `1`, usando `SMOTE`, uma vez que  negativo ocorre em mais de 90% dos casos do atributo `diagnostico_diabetes` |
| `Streamlit` | Framework de frontend, com foco em modelos em produção e prototipagem | Criar o frontend da aplicação web, para melhor experiência do usuário |
| `Joblib` | Biblioteca de conjunto de ferramentas para fornecer pipelines leves | Salvar o modelo mais eficiente para poder usá-lo na aplicação web |

## Aonde o projeto está atualmente

O modelo feito com XGBoost e predict_proba já está pronto. As Análises Exploratórias dos Dados estão sendo aprimoradas com histogramas com Curva Normal e KDE, para maior entendimento da evolução dos dados, e boxplot, para visualização e posterior tratamento de outliers.

## Próximos passos

1. Conclusão das `Análises Exploratórias dos Dados`
2. Criação, treino e testes de novos modelos, como `Logistic Regression`, para determinar qual o melhor e salvá-lo em `.pkl` (picle, Joblib)
3. Criação da aplicação web, à partir do frontend com `Streamlit` e o modelo no formato `.pkl`
4. Testes da aplicação e usar o projeto na `Streamlit Community Cloud`

## Muito obrigado por sua visita ao repositório!
