# 📝 Manual de Instruções para Uso do ChatGPT Personalizado

## 1️⃣ Carregar o Contrato
- **Ação:** 
  - Suba o arquivo `.docx` no **Cverino dos Contratos**, garantindo que todas as variáveis corretas estejam inseridas.
- **Integração com ChatGPT:** 
  - O ChatGPT verifica o conteúdo do contrato e identifica se estão faltando variáveis ou se há dados ausentes. Ele pode sugerir variáveis adicionais com base no contexto do contrato.
- **Exemplo de Uso:** 
  - Ao subir um contrato de compra e venda, o ChatGPT sugere a adição de variáveis como `${[[CLIENTE][NOME]]}` e `${[[FORMA_DE_PAGAMENTO]]}` caso estejam ausentes.

---

## 2️⃣ Verificar Erros
- **Ação:** 
  - O Cverino detecta automaticamente erros em variáveis mal formatadas ou não preenchidas.
- **Integração com ChatGPT:** 
  - O ChatGPT sugere correções de forma proativa, mostrando exemplos e oferecendo opções rápidas para resolver os problemas.
- **Exemplo de Uso:** 
  - Se uma variável como `${[[CLIENTE][CPF]]}` estiver faltando, o ChatGPT sugere: 
    > "A variável do CPF está ausente. Deseja incluí-la automaticamente?"

---

## 3️⃣ Facilitar Repetições e Condicionais
- **Ação:** 
  - Utilize condicionais e repetições, como `${SE_ASSOCIADO_N_TIPO_ASSOCIADO_M}...${/SE_ASSOCIADO_N_TIPO_ASSOCIADO_M}`, para automatizar o preenchimento de múltiplos associados ou unidades.
- **Integração com ChatGPT:** 
  - O ChatGPT ajuda a configurar essas repetições de forma automática, criando blocos de variáveis repetidos conforme a necessidade do contrato.
- **Exemplo de Uso:** 
  > "Deseja que eu configure automaticamente blocos para 5 associados? Usarei as condicionais `${SE_ASSOCIADO_1_TIPO_ASSOCIADO_1}`, `${SE_ASSOCIADO_2_TIPO_ASSOCIADO_1}`, etc."

---

## 4️⃣ Consultar Variáveis Existentes
- **Ação:** 
  - Sempre que precisar preencher um campo no contrato, consulte as variáveis documentadas no sistema.
- **Integração com ChatGPT:** 
  - Ao receber uma pergunta, o ChatGPT irá verificar os documentos categorizados para localizar a variável correta.
- **Exemplo de Uso:** 
  - Para inserir o nome do associado, utilize `${[[ASSOCIADO][NOME]]}`, conforme documentado.

---

## 5️⃣ Lidar com Variáveis Faltantes
- **Ação:** 
  - Se uma variável não for encontrada, o ChatGPT informará que ela não existe no sistema.
- **Exemplo de Resposta:**
  > "A variável solicitada não está documentada. Consulte os documentos para verificar as variáveis disponíveis."
  
- **Alternativa:** 
  - Se houver uma variável semelhante, o ChatGPT poderá sugerir uma alternativa próxima, deixando claro que é apenas uma aproximação.

---

## 6️⃣ Atualizar Variáveis
- **Ação:** 
  - Sempre que houver mudanças ou atualizações nos documentos, é importante manter o ChatGPT atualizado com as novas variáveis.
- **Integração com ChatGPT:** 
  - O assistente poderá ser atualizado para refletir novas variáveis ou alterações em documentos, sem comprometer as instruções previamente definidas.

---

## 7️⃣ Exemplos de Uso
### Pergunta:
> "Como posso inserir a condição de pagamento no contrato?"

### Resposta Correta:
> "Para inserir a condição de pagamento, utilize `${[[FORMA_DE_PAGAMENTO]]}`, conforme documentado."

---

## 🔄 Atualizações Futuras
- À medida que novos documentos ou versões das variáveis forem adicionados ao sistema, este manual deverá ser atualizado para refletir essas mudanças e garantir a conformidade das respostas geradas pelo ChatGPT.
