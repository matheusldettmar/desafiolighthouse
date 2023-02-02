# desafiolighthouse
Os pacotes necessários e suas respectivas versões podem ser encontrados no arquivo 'requirements.txt'.

É necessário os arquivos desafio_manutencao_preditiva_teste.csv e desafio_manutencao_preditiva_treino.csv

Cada rodada de testes o modelo salva um arquivo csv com as métricas de avaliação para cada categoria. O nome do arquivo está no formato método_tratamento.csv.

O ultimo modelo do codigo modelo_lighthouse.ipynb (aba: SVM com SMOTE oversampling e class weight FINAL) salva um arquivo chamado 'predicted.csv' que consiste em uma planilha com apenas duas colunas (rowNumber, predictedValues). 

Após rodar a aba 'Importações' no arquivo modelo_lighthouse.ipynb cada aba de cada tentativa de ajuste da base de treino (como Oversampling ou Undersampling) pode ser rodada separadamente.

Como a natureza do problema envolve detecção de falhas é mais interessante que o modelo não deixe de indentificar as falhas, mesmo que com uma precisão não ideal, do que apontar que um equipamento prestes a falhar não falhará. Portanto a métrica escolhida para a comparação dos modelos é o Recall. 