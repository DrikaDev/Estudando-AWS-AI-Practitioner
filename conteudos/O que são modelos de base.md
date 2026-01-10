## O que são Modelos de Base / Fundação?

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

## Ciclo de Vida de um Modelo de Base / Fundação (Foundation Model – FM)

Os **Modelos de Base / Fundação (Foundation Models – FMs)** passam por diferentes estágios ao longo do seu ciclo de vida, desde a criação até o uso contínuo 
em produção.

### 1. Treinamento (Pré-treinamento)

Neste estágio, o modelo é treinado com **grandes volumes de dados diversos**, geralmente pelo provedor do modelo (ex.: Amazon, Anthropic, Meta).

#### Características:
- Aprendizado geral e não especializado
- Alto custo computacional
- Executado pelo provedor do modelo
- Usuários finais normalmente **não participam** desse estágio

### 2. Ajuste do Modelo (Customization)

Após o pré-treinamento, o modelo pode ser ajustado para casos de uso específicos.

#### Formas de ajuste:
- **Prompt engineering**
- **Fine-tuning** com dados específicos

#### Objetivo:
- Adaptar o comportamento do modelo
- Melhorar a relevância das respostas para um domínio específico

### 3. Implantação (Deployment)

O modelo ajustado é disponibilizado para uso em ambientes de produção.

#### Características:
- Exposição do modelo via API
- Integração com aplicações
- Gerenciamento de acesso e segurança
- Escalabilidade gerenciada pela plataforma (ex.: Amazon Bedrock)

### 4. Monitoramento e Avaliação Contínua

Após a implantação, o modelo precisa ser continuamente monitorado para garantir qualidade e comportamento esperado.

#### O que é avaliado:
- Respostas inesperadas
- Novos padrões de dados
- Qualidade ao longo do tempo
- Possível drift de dados ou comportamento

#### Objetivo:
- Garantir desempenho consistente
- Identificar a necessidade de ajustes futuros

## Resumo do Ciclo de Vida

```text
Treinamento → Ajuste → Implantação → Monitoramento Contínuo
```

