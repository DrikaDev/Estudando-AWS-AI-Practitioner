## Modificação de Pesos em um Grande Modelo de Linguagem (LLM)

Em modelos de linguagem (LLMs), **os pesos (weights)** são **os parâmetros que determinam como o modelo transforma entradas em saídas**.  

Modificar os pesos significa **ajustar esses parâmetros para melhorar o desempenho ou adaptar o modelo a tarefas específicas**.

## 🧠 Como funciona

1. **Entrada (input)**  
   - Exemplo: `"O céu é ____"`  
   - O modelo tenta prever a próxima palavra, ex.: `"azul"`.

2. **Previsão e cálculo de erro**  
   - O modelo gera uma saída.  
   - Calcula-se a **diferença entre a previsão e a saída correta** (função de perda).

3. **Backpropagation e otimização**  
   - A diferença gera **gradientes**, indicando como cada peso deve ser ajustado.  
   - **Gradient Descent** (ou variantes, como Adam) ajusta os pesos para reduzir a perda.

## 🔧 Métodos de modificação de pesos em LLMs

| Método | Descrição | Quando usar |
|--------|-----------|------------|
| **Fine-Tuning Completo (Ajuste Fino)** | Treina um modelo existente com um **conjunto de dados específico** para melhorar desempenho em uma tarefa ou domínio. Ele **altera os pesos internos do modelo**. | Quando há muitos dados e recursos de GPU/CPU disponíveis |
| **LoRA (Low-Rank Adaptation)** | Adiciona **pequenas matrizes** que modificam os efeitos dos pesos originais | Adaptar o modelo a uma tarefa específica sem treinar tudo |
| **Prompt Tuning / Prefix Tuning** | Treina **vetores especiais de entrada** que influenciam a saída, sem alterar pesos originais | Poucos dados ou economia de recursos |
| **Adapters** | Pequenos módulos inseridos entre camadas do modelo | Personalização sem alterar o modelo principal |

> ⚡ **Resumo:** os pesos só mudam através de **backpropagation/otimização**, seja ajustando o modelo inteiro ou adicionando adaptadores específicos.

---

## 📈 Por que isso importa?

- Permite **personalizar o modelo** para tarefas específicas.  
- **Reduz tempo de desenvolvimento**, já que o modelo aprende com menos dados ou de forma mais eficiente.  
- Mantém o modelo **flexível e escalável**, sem precisar treinar tudo do zero.

---

## 🔗 Referências

- [Backpropagation e Gradient Descent](https://en.wikipedia.org/wiki/Backpropagation)  
- [Fine-Tuning de LLMs](https://huggingface.co/docs/transformers/training)  
- [LoRA: Low-Rank Adaptation](https://arxiv.org/abs/2106.09685)  
- [Prompt Tuning](https://arxiv.org/abs/2104.08691)
