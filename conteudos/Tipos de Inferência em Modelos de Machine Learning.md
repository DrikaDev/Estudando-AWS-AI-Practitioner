## Tipos de Inferência em Modelos de Machine Learning

Este documento explica a diferença entre **inferência assíncrona** e **inferência sem servidor** usando exemplos fáceis do dia a dia.

## Mas o que são **"Inferências"** em Machine Learning?

**Inferência** é o processo em que um **modelo de Machine Learning utiliza o conhecimento que aprendeu durante o treinamento para gerar uma resposta, 
previsão ou decisão**.  

Em outras palavras:  

> **Inferência é usar um modelo já treinado para responder a novos dados.**

## 🌱 Exemplo simples do dia a dia

Imagine que você aprendeu a reconhecer frutas:

- Você viu várias maçãs e bananas (fase de treinamento).
- Depois, alguém te mostra uma fruta nova.
- Você diz: “Isso é uma maçã”.

➡️ Esse ato de reconhecer é a **inferência**.

## 💻 Exemplo em Machine Learning

1. Um modelo é **treinado** para identificar e-mails de spam.
2. Um novo e-mail chega.
3. O modelo classifica o e-mail como:
   - **Spam** ❌  
   - **Não é spam** ✅  

➡️ Essa classificação é uma **inferência**.

## 🔄 Treinamento vs Inferência

| Fase | O que acontece |
|----|--------------|
| **Treinamento** | O modelo aprende ajustando seus pesos internos |
| **Inferência** | O modelo usa os pesos aprendidos para gerar respostas |

> ⚠️ Importante:  
> Durante a **inferência**, os pesos do modelo **não são alterados**.

## 🤖 Inferência em Grandes Modelos de Linguagem (LLMs)

Quando você faz uma pergunta para um LLM, como:

> “O que são inferências em Machine Learning?”

O modelo:
1. Recebe o texto de entrada (*input*).
2. Processa a informação usando seus pesos treinados.
3. Gera uma resposta em texto (*output*).

➡️ Cada resposta gerada por um LLM é uma **inferência**.

## 🧩 Tipos comuns de inferência

- **Inferência em tempo real**: resposta imediata (ex.: chatbots, APIs)
- **Inferência assíncrona**: resposta gerada posteriormente (ex.: processamento em lote)
- **Inferência em lote**: vários dados processados de uma só vez
- **Inferência sem servidor (serverless)**: escala automática sem gerenciamento de infraestrutura

## 🧠 Para memorizar

> **Treinar é ensinar o modelo.  
Inferir é fazer o modelo responder.**

## 🔁 Inferência Assíncrona

### Conceito
- Ideal para **workloads grandes**, com payloads de até **1 GB** ou processamento de até **1 hora**.
- Indicada para **processamento em lote**, quando **não é necessária resposta imediata**.
- O trabalho é enviado, processado em segundo plano e o resultado é recuperado depois.

### Exemplo simples
**Máquina de lavar roupas**:
- Você coloca as roupas na máquina.
- Ela trabalha sozinha por um tempo.
- Você não fica esperando.
- Depois, volta para buscar o resultado.

### Exemplo prático
- Análise de **centenas de PDFs**
- Processamento de logs
- Pré-processamento de grandes volumes de dados

### Quando usar
- Dados grandes (MB ou GB)
- Processamento demorado
- Trabalho em lote
- Tempo de resposta não crítico

## ⚡ Inferência Sem Servidor (Serverless)

### Conceito
- Ideal para workloads com **tráfego imprevisível** e períodos ociosos.
- **Não exige gerenciamento de infraestrutura**.
- Escala automaticamente conforme a demanda.
- Indicada para **respostas quase em tempo real**.

### Exemplo simples
**Fast-food**:
- Você faz o pedido.
- Recebe rapidamente.
- Se chegar mais gente, o sistema se adapta sozinho.

### Exemplo prático
- Chatbots
- Autocomplete
- APIs de previsão
- Aplicações web com usuários variáveis

### Quando usar
- Respostas rápidas
- Tráfego imprevisível
- Aplicações quase em tempo real
- Sem gerenciamento de servidores

## 🔍 Comparação rápida

| Situação | Tipo de inferência |
|--------|-------------------|
| Processar arquivos grandes | Inferência assíncrona |
| Trabalho em lote | Inferência assíncrona |
| Chat ou autocomplete | Inferência sem servidor |
| API com usuários variáveis | Inferência sem servidor |

## 🧠 Para memorizar

> **Inferência assíncrona**: “processa com calma, vejo depois”  
> **Inferência sem servidor**: “responde agora, sem eu cuidar da infra”
