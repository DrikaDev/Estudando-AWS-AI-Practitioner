## Amazon Bedrock

O **Amazon Bedrock** é um serviço da AWS que permite criar aplicações com **IA generativa** (texto, imagens e código) de forma simples, segura e escalável, 
sem a necessidade de treinar, ajustar ou hospedar modelos do zero.  

Ele fornece acesso, via API, a **Modelos de Base / Fundação (Foundation Models – FMs)** totalmente gerenciados pela AWS.  

### O que são Modelos de Base / Fundação?

**Modelos de Base / Fundação** são modelos de Inteligência Artificial de **grande escala**, genéricos e poderosos, treinados com **grandes volumes
de dados variados**, capazes de executar **múltiplas tarefas diferentes**.

Eles não são criados para resolver apenas um problema específico, são criados para servir como uma **base reutilizável** para diversas aplicações.

- Modelos de Base / Fundação são acessados pelo **Amazon Bedrock**
- Não é necessário treinar modelos do zero
- O acesso é feito via API
- O comportamento pode ser ajustado com:  
  - **Prompt engineering** - melhorar a forma como você faz a pergunta ao modelo. Exemplo:  
        - ❌ Prompt ruim: - “Fale sobre esqui”  
        - ✅ Prompt bem feito: “Explique esqui na neve, em montanhas, não esqui aquático, com foco em turismo.”  
  - **Fine-tuning** - ajustar o modelo com seus próprios dados, fornecendo exemplos, ajustando pesos do modelo, tornando o modelo mais especializado. Exemplo:  
        - Treinar o modelo com milhares de exemplos de:  
            - textos de turismo  
            - imagens de esqui na neve  

> Prompt primeiro, fine-tuning só quando o prompt não resolve.

## O que é possível fazer com o Amazon Bedrock?

### ✍️ Geração de texto
- Chatbots
- Resumos de documentos
- Respostas automáticas
- Análise e classificação de texto

### 🖼️ Geração de imagens
- Conteúdo para marketing
- Design e ilustrações
- Criação de imagens a partir de descrições textuais

### 💻 Geração de código
- Trechos de código
- Explicações técnicas
- Suporte à automação

## Principais benefícios

### ✅ Não é necessário treinar modelos
Utiliza modelos de fundação prontos para uso.

### ✅ Segurança e privacidade
- Integração com **IAM**, **VPC** e **KMS**
- Os dados do cliente não são usados para treinar os modelos

### ✅ Escalabilidade automática
A AWS gerencia toda a infraestrutura por trás do serviço.

### ✅ Flexibilidade
Permite trocar modelos sem grandes mudanças no código da aplicação.

## Arquitetura simplificada

```text
Aplicação → Amazon Bedrock → Modelo de IA → Resposta
```
A aplicação envia um prompt e recebe a resposta gerada pelo modelo.

---

## Geração de imagens no Amazon Bedrock usando Prompt Negativo

Uma empresa de turismo usa o Amazon Bedrock para produzir imagens de pessoas esquiando na neve para uma futura campanha de marketing.  
O modelo está gerando imagens de pessoas praticando esqui aquático, além de esqui na neve.  
A empresa não deseja imagens de esqui aquático.

**Pergunta:**  
Que opção a empresa teria para evitar a geração de imagens indesejadas com o **MENOR esforço operacional**?

---

## Resposta

Utilizar **prompt negativo (negative prompting)** para restringir a geração de conteúdos indesejados.

---

## Explicação

É possível usar um prompt negativo para instruir o modelo sobre conceitos, imagens ou elementos que **não devem** ser incluídos na saída.  
Nesse caso, o prompt pode especificar explicitamente que imagens de esqui aquático não devem ser geradas, reduzindo a necessidade de ajustes complexos ou re-treinamento do modelo.

Essa abordagem oferece o **menor esforço operacional**, pois não exige fine-tuning, mudanças de infraestrutura ou pós-processamento das imagens.

---

## Exemplo de prompt

> “Generate images of people skiing on snow in mountains, **not water skiing**, **no boats**, **no lakes**, **no ocean**.”
