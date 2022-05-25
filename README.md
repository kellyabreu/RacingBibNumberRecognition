# RacingBibNumberRecognition

### 1. Os links para as imagens encontram-se nos algoritmos.

### 2. Sugestão de melhoria: artigo fpls-11-00898.pdf.

### 3. Resultados obtidos (necessário atualizar):

https://docs.google.com/spreadsheets/d/1sN1ciGKkFqZsd9GWKvCaVYjPZOA19wpICjlDjcmfqqE/edit?usp=sharing

F1 Score = 2*((precision * recall) / (precision + recall)

| NOVOS TESTES                                                                           |           |        |              |           |             |
| -------------------------------------------------------------------------------------- | --------- | ------ | ------------ | --------- | ----------- |
| 1 -Teste apenas com imagens Noturnas - Universidade de Barcelona (flip-rotação-brilho) |           |        |              |           |             |
| MODELO                                                                                 | Precision | Recall | F1-Score     | Algoritmo | Batch/Epoch |
| yolov4                                                                                 | 0,47      | 0,24   | 0,3177464789 | Darknet   | 2000        |
| yolov5                                                                                 | 0,23      | 0,36   | 0,2806779661 | Pytorch   | 100         |
| retinaNet                                                                              | 0,46      | 0,52   | 0,4881632653 | Pytorch   | 24          |
|                                                                                        |           |        |              |           |             |
| 2 - IMAGENS NOTURNAS + DIURNAS (FULL) (rotação-brilho)                                 |           |        |              |           |             |
| MODELO                                                                                 | Precision | Recall | F1-Score     | Algoritmo | Batch/Epoch |
| yolov4                                                                                 | 0,57      | 0,63   | 0,5985       | Darknet   | 2000        |
| yolov5                                                                                 | 0,86      | 0,44   | 0,5821538462 | Pytorch   | 299         |
| retinaNet                                                                              | 0,77      | 0,8    | 0,7847133758 | Pytorch   | 37          |
|                                                                                        |           |        |              |           |             |
| 3 -Teste FULL sem imagens Noturnas BR (rotação-brilho)                                 |           |        |              |           |             |
| MODELO                                                                                 | Precision | Recall | F1-Score     | Algoritmo | Batch/Epoch |
| yolov4                                                                                 | 0,64      | 0,71   | 0,6731851852 | Darknet   | 2000        |
| yolov5                                                                                 | 0,98      | 0,76   | 0,856091954  | Pytorch   | 204         |
| retinaNet                                                                              | 0,68      | 0,75   | 0,7132867133 | Pytorch   | 17          |

| TESTES ANTERIORES                                           |           |        |              |             |
| ----------------------------------------------------------- | --------- | ------ | ------------ | ----------- |
| 1 - IMAGENS NOTURNAS + DIURNAS (FULL) (flip-rotação-brilho) |           |        |              |             |
| MODELO                                                      | Precision | Recall | F1-Score     | Batch/Epoch |
| yolov4                                                      | 0,63      | 0,79   | 0,7009859155 | 2000        |
| yolov5                                                      | 0,82      | 0,65   | 0,725170068  | 100         |
| retinaNet                                                   | 0,76      | 0,86   | 0,8069135802 | 37          |
|                                                             |           |        |              |             |
| 2 - IMAGENS NOTURNAS (flip-rotação-brilho)                  |           |        |              |             |
| MODELO                                                      | Precision | Recall | F1-Score     | Batch/Epoch |
| yolov4                                                      | 0,08      | \-     | \-           | 2000        |
| yolov5                                                      | 0,16      | \-     | \-           | 100         |
| retinaNet                                                   | \-1       | \-1    | \-           | 37          |
