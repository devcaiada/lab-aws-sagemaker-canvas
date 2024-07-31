# 📊 Previsão Admissão Universidade com AWS com [SageMaker Canvas](https://aws.amazon.com/pt/sagemaker/canvas/)

Desafio DIO - Bootcamp Nexa - Machine Learning para Iniciantes na AWS - utilizando o SageMaker Canvas.


## 🚀 Passo a Passo

### 1. Selecionar Dataset

- Foi selecionado o dataset university_admission que mostra a performance de alunos durante o colégio e a probabilidade de admissão em uma universidade.

### 2. Construir/Treinar

- Após importar o dataset, criei um modelo de treinamento e defini a coluna alvo (Chance_of_Admission) para ser prevista pelo modelo, conforme mostra imagem abaixo:

![target_column](https://github.com/devcaiada/lab-aws-sagemaker-canvas/blob/main/assets/target%20column.png?raw=true)

* O processo selecionado foi o QuickBuild, que leva de 10 a 15 minutos para treinar o modelo.

### 3. Analisar

-   Após o treinamento, essas foram as métricas encontradas e seus impactos na análise de dados.

![quick_build](https://github.com/devcaiada/lab-aws-sagemaker-canvas/blob/main/assets/quick%20build.png?raw=true)

* Como podemos observar, as métricas CGPA, com 43,47% e GRE_Score com 20,67%, são as que mais afetam a probabilidade de admissão universitária.

* CGPA (Grade Points Average) - É a media de notas e desempenho de um aluno durante o ensino médio.

* GRE Score (Graduate Record Examination) - Fazendo uma analogia simples, seria como o nosso ENEM no Brasil.

### 4. Prever

 * através do modelo podemos notar que quanto maior a nota CGPA, maior a probabilidade de um aluno ser admitido na universidade.

 ![cgpa_impact](https://github.com/devcaiada/lab-aws-sagemaker-canvas/blob/main/assets/GPA%20impact.png?raw=true)

 * Logo abaixo temos algumas métricas avançada:

 ![advance_metrics](https://github.com/devcaiada/lab-aws-sagemaker-canvas/blob/main/assets/Advance%20metrics.png?raw=true)

 * R2 (R Quadrado) - métrica que indica o quanto a linha de regressão se ajusta aos dados.

 * MAE (Erro Médio Absoluto) - Esta é uma métrica bem simples para verificar a acurácia do modelo. Ela é medida na mesma unidade da variável dependente e não é sensível a outliers, ou seja, valores muito extremos não vão impactar esta métrica em uma escala intensificada.

 * RMSE (Raíz do Erro Quadrático Médio) - Calcula o quão próximo os pontos de dados reais estão dos valores previstos pelo modelo e é usado para medir o desvio padrão dos resíduos.

## 🚨 IMPORTANTE

Após concluir a análise, lembre-se de fazer logout do seu modelo no SageMaker. Deixar o domínio aberto pode resultar em custos e complicações para resolver essas cobranças na plataforma.

FAÇA LOGOUT!

![logout](https://github.com/devcaiada/lab-aws-sagemaker-canvas/blob/main/assets/loggout.png?raw=true)

---
