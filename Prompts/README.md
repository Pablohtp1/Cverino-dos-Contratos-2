# 🚀 Manual de Uso de Prompts no Cverino dos Contratos

## Introdução
Este manual explica como utilizar **prompts** no **Cverino dos Contratos** para automação eficiente no preenchimento de contratos utilizando **variáveis documentadas**. O objetivo é permitir a execução automatizada de tarefas como preenchimento de dados do associado, assinaturas eletrônicas, dados de faturamento, empreendimentos, imobiliárias e cessão de direitos.

---

## O que são Prompts?

**Prompts** são comandos que utilizam **variáveis documentadas** no Cverino dos Contratos para preencher, verificar e ajustar contratos automaticamente. Eles permitem automatizar campos como informações de associados, assinaturas eletrônicas e dados de faturamento, garantindo precisão e velocidade na execução de contratos.

---

## 🎯 Como Criar um Prompt Eficiente Usando Variáveis

### 1. **Use as Variáveis Certas**
Sempre utilize as variáveis documentadas para garantir que os dados serão preenchidos corretamente no contrato. Para cada área do contrato, existe um conjunto específico de variáveis.

- **Exemplo**: _"Preencha o contrato com as variáveis ${[[ASSOCIADO][1][NOME]]}, ${[[ASSOCIADO][1][PROFISSAO]]}, e ${[[ASSOCIADO][1][DOCUMENTO]]} para o associado."_

### 2. **Instruções Claras e Condicionais**
Utilize condicionais quando necessário para gerar partes dinâmicas do contrato. Por exemplo, se o associado for de um tipo específico, preencha as informações relacionadas.

- **Exemplo**: _"Utilize ${SE_ASSOCIADO_1_TIPO_ASSOCIADO_1} para definir o tipo do associado e inserir os dados conforme ${[[ASSOCIADO][1][NOME]]}, ${[[ASSOCIADO][1][RG]]} e ${[[ASSOCIADO][1][DOCUMENTO]]}."_

### 3. **Preencher e Verificar Campos**
Além de preencher, você pode usar prompts para verificar se as variáveis foram corretamente aplicadas. Caso estejam ausentes, o sistema pode preencher automaticamente ou alertar para correção.

- **Exemplo**: _"Verifique se o contrato contém ${[[FATURAMENTO][1][NOME]]}, ${[[FATURAMENTO][1][CPF]]}, e ${[[FATURAMENTO][1][ENDERECO]]}. Caso algum esteja vazio, adicione os valores padrão."_

---

## 🛠️ Exemplos Práticos de Prompts Usando Variáveis no Cverino

### 1. **Associados com Condicionais**
   _"Gere informações de qualificação para associados usando o prompt condicional ${SE_ASSOCIADO_1_TIPO_ASSOCIADO_1}. Nome: ${[[ASSOCIADO][1][NOME]]}, Nacionalidade: ${[[ASSOCIADO][1][NACIONALIDADE]]}, Estado Civil: ${[[ASSOCIADO][1][ESTADO_CIVIL]]}, Profissão: ${[[ASSOCIADO][1][PROFISSAO]]}, RG: ${[[ASSOCIADO][1][RG]]}, Órgão Emissor: ${[[ASSOCIADO][1][RG_ORGAO_EMISSOR]]}, CPF: ${[[ASSOCIADO][1][DOCUMENTO]]}."_

   - **O que faz**: O sistema gera automaticamente os dados do associado 1, com base nas variáveis documentadas, apenas se a condição para o tipo de associado for verdadeira.

### 2. **Assinaturas Eletrônicas**
   _"Insira as assinaturas eletrônicas com ${[[ASSINATURA_ELETRONICA][ASSINATURA_CLIENTE]]} para o cliente e ${[[ASSINATURA_ELETRONICA][1][ASSINATURA_ASSOCIADO]]} para o associado 1."_

   - **O que faz**: O sistema preenche automaticamente as assinaturas eletrônicas necessárias no contrato, garantindo que todos os campos estejam prontos para assinatura digital.

### 3. **Dados de Faturamento**
   _"Preencha os dados de faturamento usando ${[[FATURAMENTO][1][NOME]]}, ${[[FATURAMENTO][1][CPF]]}, ${[[FATURAMENTO][1][ENDERECO]]}, e ${[[FATURAMENTO][1][BANCO]]}."_

   - **O que faz**: O sistema insere automaticamente os dados de faturamento, como nome, CPF, endereço e banco do cliente, com base nas variáveis configuradas.

### 4. **Dados do Empreendimento**
   _"Insira os dados do empreendimento, como nome (${[[EMPREENDIMENTO][NOME]]}), data de entrega (${[[EMPREENDIMENTO][DATA_ENTREGA]]}), área construída (${[[EMPREENDIMENTO][AREA_CONSTRUIDA]]}), e localização (${[[EMPREENDIMENTO][CIDADE]]}, ${[[EMPREENDIMENTO][ESTADO]]})."_

   - **O que faz**: O sistema preenche automaticamente as informações do empreendimento no contrato, garantindo que o nome, a data de entrega e a localização estejam corretamente inseridos.

### 5. **Cessão de Direitos**
   _"Preencha os dados da cessão de direitos utilizando as variáveis ${[[CLIENTE_CESSAO][NOME]]}, ${[[CLIENTE_CESSAO][DOCUMENTO]]}, e ${[[CLIENTE_CESSAO][NACIONALIDADE]]}."_

   - **O que faz**: O sistema insere automaticamente os dados do cliente da cessão de direitos, como nome, CPF/CNPJ e nacionalidade, conforme as variáveis documentadas.

---

## 💡 Dicas para Uso Eficiente de Prompts com Variáveis

1. **Utilize Condicionais para Associados**
   Ao trabalhar com múltiplos associados, use condicionais para garantir que as variáveis corretas sejam aplicadas de acordo com o tipo de associado.

   - **Exemplo**: _"Use ${SE_ASSOCIADO_1_TIPO_ASSOCIADO_1} para aplicar variáveis específicas do associado 1 no contrato."_

2. **Automatize Assinaturas Eletrônicas**
   Sempre que possível, insira as variáveis de assinatura eletrônica de forma automática para garantir que todas as partes do contrato assinem corretamente.

   - **Exemplo**: _"Utilize ${[[ASSINATURA_ELETRONICA][ASSINATURA_CLIENTE]]} para o cliente e ${[[ASSINATURA_ELETRONICA][1][ASSINATURA_ASSOCIADO]]} para o associado 1."_

3. **Verifique a Compleção dos Campos**
   Use prompts para verificar se todas as variáveis importantes foram aplicadas, como dados de faturamento ou do empreendimento.

   - **Exemplo**: _"Verifique se as variáveis ${[[FATURAMENTO][1][NOME]]} e ${[[EMPREENDIMENTO][NOME]]} estão presentes antes de finalizar o contrato."_

---

## Como Funciona o Processo de Resposta com Variáveis

Ao utilizar prompts no **Cverino dos Contratos**, o sistema processa automaticamente as variáveis documentadas, preenchendo os campos de acordo com as instruções fornecidas. Ele pode:

- **Preencher automaticamente** dados de associados, assinaturas eletrônicas e informações de empreendimentos.
- **Verificar campos faltantes** e sugerir o preenchimento de informações padrão.
- **Ajustar dados de faturamento** e realizar a inserção de múltiplos associados com base nas variáveis disponíveis.

---

## Conclusão

O uso de **prompts** no **Cverino dos Contratos** permite uma automação eficiente e rápida de contratos, garantindo que todas as variáveis sejam corretamente aplicadas e verificadas. Utilizando as variáveis documentadas corretamente, você pode garantir que seus contratos sejam preenchidos de forma precisa e automatizada, economizando tempo e evitando erros.
