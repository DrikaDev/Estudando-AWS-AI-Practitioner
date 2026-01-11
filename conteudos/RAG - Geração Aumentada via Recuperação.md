## RAG - Geração Aumentada via Recuperação

A **Geração Aumentada via Recuperação (RAG, do inglês *Retrieval-Augmented Generation*)** é uma técnica que **combina grandes modelos de linguagem (LLMs) 
com fontes externas de informação** para gerar respostas mais precisas, relevantes e atualizadas.

## 1️⃣ O que significa "Recuperação"?

No contexto da RAG, **recuperação** refere-se ao processo pelo qual o modelo:

- Consulta **fontes externas confiáveis** (bases de conhecimento, documentos internos, APIs, etc.).  
- Usa essas informações para **complementar ou corrigir seu próprio conhecimento**, além dos dados de treinamento.  

> Ou seja, mesmo que o LLM **não tenha visto algo durante seu treinamento**, ele pode **recuperar informações externas** e gerar respostas precisas.

## 2️⃣ Como funciona a RAG?

1. O modelo recebe uma **pergunta ou instrução**.  
2. Antes de gerar a resposta, ele **busca dados relevantes em uma base confiável**.  
3. Usa essas informações **como contexto adicional** para gerar a **resposta final**.

**Exemplo prático:**  

- Pergunta: `"Qual é o procedimento de segurança atualizado da minha empresa para acesso remoto?"`  
- LLM sozinho: poderia gerar uma resposta genérica.  
- LLM com RAG: **consulta a base interna da empresa** e gera uma resposta **precisa e atualizada**.

## 3️⃣ Benefícios da RAG

- 🌐 **Atualização contínua:** acessa informações que mudam rapidamente sem re-treinamento.  
- 💰 **Economia de recursos:** não é necessário treinar ou fine-tunar o LLM para cada nova base de conhecimento.  
- 🏢 **Domínio específico:** aplica LLMs a contextos internos ou especializados.  
- ✅ **Precisão e relevância:** melhora a confiabilidade das respostas do modelo.

## 4️⃣ Fluxo resumido

Pergunta do usuário
│
▼
Recuperação → Busca em base confiável
│
▼
Geração pelo LLM com contexto externo
│
▼
Resposta final precisa e atualizada

> Em outras palavras, **RAG combina “memória” do modelo + consulta externa**, garantindo que ele não dependa apenas do que aprendeu no treinamento.
