Projeto Final do Curso de Ciência de Dados | EBAC | PEDRO THOMAZ RAMOS MATTANA VIEIRA
O case escolhido foi o de predição para diagnósticos de pacientes de hipertireoidismo.

Neste projeto foi desenvolvido um modelo de machine learning para a predição de hipertireoidismo
a partir de dados clínicos e laboratoriais, com foco na correta identificação dos casos positivos. 

Inicialmente, realizou-se uma análise exploratória dos dados, que evidenciou forte desbalanceamento
da variável alvo, bem como a elevada relevância dos marcadores hormonais TSH, FTI, TT4 e T3.
A análise bivariada demonstrou que TSH e FTI apresentam maior poder discriminativo, enquanto o T4U, 
isoladamente, mostrou baixa capacidade de separação entre as classes.

Com base nesses achados, foi adotado o algoritmo XGBoost, devido à sua robustez a outliers,
capacidade de modelar relações não lineares e bom desempenho em bases desbalanceadas.
O pré-processamento incluiu imputação de valores ausentes por mediana e separação estratificada
dos dados, evitando vazamento de informação. O modelo foi avaliado utilizando métricas adequadas
ao contexto clínico, como recall, F1-score, matriz de confusão e AUC-ROC.

Os resultados obtidos foram expressivos, com AUC de aproximadamente 0,99, indicando excelente
capacidade de discriminação entre indivíduos com e sem hipertireoidismo. A matriz de confusão
revelou alta sensibilidade (98%) para a classe positiva, com número reduzido de falsos negativos,
aspecto fundamental em cenários de triagem médica. A análise de importância das variáveis
confirmou a predominância do TSH e do FTI como principais preditores, em concordância com a literatura médica.

Dessa forma, conclui-se que o modelo proposto apresenta elevado potencial como ferramenta de apoio à
triagem clínica do hipertireoidismo, podendo auxiliar profissionais de saúde na identificação precoce
da doença. Ressalta-se, entretanto, que o modelo não substitui o diagnóstico médico,
devendo ser utilizado como suporte à decisão clínica.
