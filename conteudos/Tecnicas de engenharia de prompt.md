## 📝 Técnicas de Engenharia de Prompt (Prompt Engineering)

A **engenharia de prompt** é a prática de **escrever e estruturar entradas (prompts) para modelos de linguagem (LLMs)** de forma que eles gerem **respostas mais precisas, 
úteis e relevantes**.

Existem várias técnicas que os desenvolvedores e pesquisadores usam. Aqui está um resumo completo:

## 1️⃣ Instrução clara e direta (Instruction Prompting)

- Diga explicitamente o que você quer que o modelo faça.  
- Evite ambiguidade.  

**Exemplo:**  
```text
Escreva um resumo de 3 linhas sobre o aquecimento global.
```

## 2️⃣ Exemplos (Few-Shot Prompting)

- Forneça exemplos de entrada e saída antes de pedir a resposta.  
- Ajuda o modelo a entender o formato e estilo esperado.  
Exemplo:  
```text
Traduza os seguintes textos para francês:
1. "Olá" -> "Bonjour"
2. "Como você está?" -> "Comment ça va?"
3. "Bom dia" -> ?
```

## 3️⃣ Zero-Shot Prompting

- Sem fornecer exemplos. Apenas instrução direta.  
- Útil quando você quer respostas rápidas ou genéricas.  
Exemplo:  
```
Liste cinco frutas vermelhas.
```

## 4️⃣ Chain-of-Thought (Cadeia de pensamento)

- Peça ao modelo que explique o raciocínio antes de dar a resposta.  
- Muito usado para problemas complexos ou matemáticos.  
Exemplo:  
```
Resolva: 23 x 47. Mostre o passo a passo.
```

## 5️⃣ Role Prompting (Assumir papéis)

- Diga ao modelo para agir como um especialista ou personagem.
- Ajuda a ajustar o tom e a autoridade da resposta.
Exemplo:
```
Você é um médico especialista em cardiologia. Explique os sintomas da hipertensão para um paciente leigo.
```

## 6️⃣ Contextualização / Background

- Dê contexto suficiente para a pergunta.
- Isso melhora a precisão e relevância.
Exemplo:
```
Você é um professor de história. Explique a Revolução Francesa para estudantes do ensino médio.
```

## 7️⃣ Prompt Templates / Estrutura

- Use modelos de prompts reutilizáveis para tarefas frequentes.
Exemplo de template:
```
[Instrução clara] + [Exemplos se necessário] + [Pergunta ou tarefa]
``` 

## 8️⃣ Controles de saída (Output Control)

- Indique formato, comprimento, estilo ou restrições.
Exemplo:
```
Liste 5 cidades brasileiras em ordem alfabética, apenas os nomes, separados por vírgula.
```

## 9️⃣ Iterative Refinement (Refinamento iterativo)

- Ajuste o prompt com base nas respostas anteriores até atingir o resultado desejado.
Exemplo:
```
Primeiro prompt: "Resuma este texto."  
Se a resposta for vaga, refinar: "Resuma este texto em 3 frases claras e objetivas."
``` 

## 1️⃣0️⃣ Funções Avançadas (Advanced Prompting)

- Combina técnicas como Chain-of-Thought + Role Prompting + Exemplos.
- Muito usado em LLMs grandes para tarefas complexas, como codificação ou análise de dados.

> ## 💡 Resumo:
> Engenharia de prompt é a arte de comunicar claramente com o modelo, dando instruções, contexto e exemplos para obter respostas mais precisas e úteis.
