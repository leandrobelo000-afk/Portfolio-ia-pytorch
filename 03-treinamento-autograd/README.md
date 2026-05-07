# Case 03: Aprendizado Automático com Autograd

Este projeto marca a transição da lógica matemática estática para o **Aprendizado de Máquina**.

## Objetivos Técnicos
* **Parâmetros Treináveis:** Uso de `requires_grad=True` para permitir que o PyTorch rastreie os gradientes.
* **Otimização:** Implementação do algoritmo **SGD (Stochastic Gradient Descent)** para ajuste automático de pesos.
* **Função de Custo:** Utilização do **MSE (Mean Squared Error)** para quantificar o erro do modelo.

## Resultados
O modelo demonstrou convergência estável, reduzindo drasticamente o erro (Loss) nas primeiras 200 épocas, validando a escolha dos hiperparâmetros (Learning Rate = 0.01).
