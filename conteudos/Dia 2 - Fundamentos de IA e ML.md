## 🔹 Dia 2 - Fundamentos de IA e ML - Parte 2

Neste dia, o foco é entender **casos de uso práticos de IA**, quando **não faz sentido usar Machine Learning**, as **principais técnicas de ML** e **qual serviço da AWS usar em cada cenário**.

---

## 💡 Casos de uso práticos de IA

A IA e o ML são úteis quando precisam:

- **Auxiliar a tomada de decisão humana**
- **Escalar soluções** que seriam inviáveis manualmente
- **Automatizar tarefas repetitivas**
- **Identificar padrões** em grandes volumes de dados

### Exemplos reais
- Detecção de fraude em transações financeiras
- Recomendação de produtos
- Reconhecimento de imagens e rostos
- Análise de sentimentos em textos
- Transcrição de áudio em texto

---

## 🚫 Quando NÃO usar Machine Learning

Nem todo problema precisa de IA ou ML.

Evite usar ML quando:
- O problema pode ser resolvido com **regras fixas simples**
- É necessário um **resultado exato e determinístico**
- O custo de implementação é maior que o benefício
- Não há **dados suficientes ou de qualidade**
- A explicabilidade total é obrigatória

📌 *Exemplo:*  
Se um desconto é sempre de 10%, não há motivo para usar ML — uma regra simples resolve.

---

## 🧠 Técnicas comuns de Machine Learning

### 🔹 Classificação
- Objetivo: atribuir uma **categoria** a um dado.
- Exemplos:
  - Spam ou não spam
  - Fraude ou não fraude
  - Aprovar ou rejeitar crédito

---

### 🔹 Regressão
- Objetivo: prever um **valor numérico contínuo**.
- Exemplos:
  - Previsão de preços
  - Estimativa de demanda
  - Previsão de vendas

---

### 🔹 Agrupamento (Clustering)
- Objetivo: **agrupar dados semelhantes** sem rótulos prévios.
- Exemplos:
  - Segmentação de clientes
  - Análise de comportamento
  - Agrupamento de perfis similares

---

## ☁️ Serviços de IA/ML da AWS

### 🔹 Amazon SageMaker
- Plataforma completa para criar, treinar e implantar modelos de ML.
- Usado quando há necessidade de **modelos personalizados**.

📌 *Exemplo:* criar um modelo próprio de previsão ou classificação.

---

### 🔹 Amazon Comprehend
- Serviço de **Processamento de Linguagem Natural (PLN)**.
- Analisa texto para:
  - Sentimento
  - Entidades
  - Idioma
  - Tópicos

📌 *Exemplo:* analisar comentários de clientes.

---

### 🔹 Amazon Transcribe
- Converte **áudio em texto** automaticamente.

📌 *Exemplo:* transcrição de reuniões, chamadas ou podcasts.

---

### 🔹 Amazon Translate
- Tradução automática de textos entre idiomas.

📌 *Exemplo:* traduzir descrições de produtos para outros países.

---

### 🔹 Amazon Rekognition
- Análise de **imagens e vídeos**.
- Detecta:
  - Objetos
  - Rostos
  - Texto em imagens
  - Atividades suspeitas

📌 *Exemplo:* reconhecimento facial ou moderação de conteúdo.

---

### 🔹 Amazon Lex
- Criação de **chatbots e assistentes conversacionais**.
- Base do Amazon Alexa.

📌 *Exemplo:* chatbot de atendimento ao cliente.

---

### 🔹 Amazon Polly
- Converte **texto em fala** natural.

📌 *Exemplo:* leitura automática de textos ou acessibilidade.

---

## 🗺️ Qual serviço usar em cada cenário?

| Cenário | Serviço AWS |
|------|------------|
| Modelo de ML personalizado | Amazon SageMaker |
| Análise de texto e sentimento | Amazon Comprehend |
| Áudio para texto | Amazon Transcribe |
| Tradução de idiomas | Amazon Translate |
| Análise de imagens e vídeos | Amazon Rekognition |
| Chatbots | Amazon Lex |
| Texto para fala | Amazon Polly |

---

## 🧠 Dica de estudo

> Para a prova, foque em **entender o problema primeiro** e depois escolher **o serviço da AWS mais adequado**, sempre com visão de negócio.

---

👉🏻 [Clique aqui para voltar ao RoadMap](https://github.com/DrikaDev/Estudando-AWS-AI-Practitioner/blob/main/conteudos/Roadmap%20de%20Estudos.md) 🗺️ 
