# Portfólio de Engenharia de IA: De Numpy a PyTorch

Este repositório documenta a evolução de um modelo de classificação linear, partindo de uma implementação manual com **Numpy** até uma versão otimizada e escalável utilizando **PyTorch**.

## Visão Geral do Projeto
O objetivo principal foi realizar a classificação de dados em uma fronteira de decisão linear, focando na transição de cálculos iterativos manuais para o paradigma de **computação tensorial**.

## Estrutura do Repositório

### [01-fundamentos-matematicos](./01-fundamentos-matematicos/)
Nesta etapa inicial, o foco foi a validação teórica da fronteira de decisão.
*   **Tecnologias:** Python, Numpy, Matplotlib.
*   **Abordagem:** Cálculo manual de pontos (`ret1, ret2, ret3`) para validação da lógica geométrica.

### [02-refatoracao-tensores](./02-refatoracao-tensores/)
Refatoração do script original para aproveitar o poder de processamento de Deep Learning.
*   **Vetorização:** Substituição do cálculo manual por `torch.matmul`, permitindo a multiplicação de matrizes em larga escala.
*   **Otimização de Memória:** Uso do gerenciador de contexto `torch.no_grad()` para desativar o rastreamento de gradientes durante a fase de validação, reduzindo drasticamente o consumo de RAM.
*   **Agnosticismo de Hardware:** Implementação de lógica de detecção automática de GPU (`cuda`), garantindo performance superior se houver hardware dedicado disponível.

## Tecnologias Utilizadas
*   **Python 3.0**
*   **PyTorch** (Tensors & Autograd)
*   **Numpy** (Processamento numérico)
*   **Matplotlib** (Visualização de dados)

---
**Desenvolvido por:** Leandro Belo de Almeida Gomes
