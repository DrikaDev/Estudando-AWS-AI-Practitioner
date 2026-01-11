## Divisão Conjunto de Dados em Machine Learning

Em Machine Learning, os conjuntos de dados são divididos em **três subconjuntos principais**: **treinamento**, **validação** e **teste**.  
Cada um possui um papel específico no desenvolvimento e avaliação de modelos.

## 🧠 Conjunto de Treinamento (Training Set)

- Utilizado para **treinar o modelo**.
- É nesse conjunto que o modelo **ajusta seus parâmetros internos (pesos)**.
- Representa a maior parte dos dados disponíveis.

**Objetivo:** ensinar o modelo a identificar padrões.

## 🔍 Conjunto de Validação (Validation Set)

- Usado para **avaliar o desempenho do modelo durante o treinamento**.
- Auxilia no **ajuste de hiperparâmetros**, como taxa de aprendizado, número de camadas, regularização, entre outros.
- Ajuda a evitar **overfitting**.

**Objetivo:** escolher a melhor configuração de modelo.

## 🧪 Conjunto de Teste (Test Set)

- Utilizado para a **avaliação final do modelo**.
- Contém dados que **não foram vistos** durante o treinamento ou validação.
- Mede o quão bem o modelo **generaliza para novos dados**.

**Objetivo:** verificar o desempenho real do modelo em dados novos.

## 🎯 Objetivo Principal de Separar os Conjuntos de Dados

O principal objetivo de utilizar **conjuntos de dados separados** em Machine Learning é garantir que o modelo:

- **Aprenda corretamente**, sem memorizar os dados (evitar *overfitting*);
- Seja **avaliado de forma justa**, usando dados que ele nunca viu;
- Consiga **generalizar bem** para novos cenários do mundo real;
- Permita **ajustes seguros** de hiperparâmetros sem comprometer a avaliação final.

Separar os dados ajuda a identificar se o modelo:
- Está apenas decorando os dados de treinamento;
- Ou realmente aprendeu padrões que funcionam em dados novos.

## 🔄 Resumo dos Conjuntos de Dados

| Conjunto | Finalidade |
|--------|-----------|
| **Treinamento** | Ajustar os parâmetros do modelo |
| **Validação** | Ajustar hiperparâmetros e avaliar durante o treino |
| **Teste** | Avaliar o desempenho final com dados não vistos |

## 🧠 Para memorizar

> **Treinamento ensina o modelo.**  
> **Validação ajusta o modelo.**  
> **Teste avalia se o modelo realmente aprendeu.**
