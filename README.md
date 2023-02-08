# desafiolighthouse
Os pacotes necessários e suas respectivas versões podem ser encontrados no arquivo 'requirements.txt'.

São necessário os arquivos desafio_manutencao_preditiva_teste.csv e desafio_manutencao_preditiva_treino.csv.

O Profile Report usado na EDA foi salvo como report_baseTreino em html, podendo ser salvo a partir do git e aberto em um browser.  

Para cada rodada de testes o modelo salva um arquivo csv com as métricas de avaliação para cada categoria. O nome do arquivo está no formato método_tratamento.csv.

O último modelo do código modelo_lighthouse.ipynb (aba: SVM com SMOTE oversampling e class weight FINAL) salva um arquivo chamado 'predicted.csv' que consiste em uma planilha com apenas duas colunas (rowNumber, predictedValues). 

Após rodar a aba 'Importações' no arquivo modelo_lighthouse.ipynb cada aba das tentativas de ajuste da base de treino (como Oversampling ou Undersampling) podem ser rodadas separadamente.

Como a natureza do problema envolve detecção de falhas é mais interessante que o modelo não deixe de indentificar as falhas, mesmo que com uma precisão não ideal, do que apontar que um equipamento prestes a falhar não falhará. Portanto a métrica escolhida para a comparação dos modelos é o Recall. 

O arquivo predicted.csv com as previsões para a base  desafio_manutencao_preditiva_teste.csv está na pasta 'output'.