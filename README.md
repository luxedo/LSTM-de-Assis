# LSTM de Assis

Código para gerar um modelo de previsão de palavras baseado nas obras de Machado de Assis utilizando Embeddings e LSTM.

O modelo é criado a partir do notebook `LSTM de Assis.ipynb` no arquivo `LSTM-de Assis.h5`. Também estão disponíveis o dicionário utilizado e o dicionário de índices. O modelo é uma rede neural com 5 camadas de acordo com a seguinte configuração:

```
Model: "LSTM-de-Assis"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
embedding (Embedding)        (1, None, 128)            3635072   
_________________________________________________________________
lstm1 (LSTM)                 (1, None, 128)            131584    
_________________________________________________________________
lstm2 (LSTM)                 (1, None, 128)            131584    
_________________________________________________________________
densa1 (TimeDistributed)     (None, None, 128)         16512     
_________________________________________________________________
densa2 (TimeDistributed)     (None, None, 28399)       3663471   
=================================================================
Total params: 7,578,223
Trainable params: 7,578,223
Non-trainable params: 0
```



## Licença

> This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
>
> This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
>
> You should have received a copy of the GNU General Public License along with this program. If not, see http://www.gnu.org/licenses/.
