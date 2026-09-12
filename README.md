#  Desafio DIO: Treinando uma IA de Aprendizagem com o NotebookLM

> **Link de acesso ao Caderno no NotebookLM:** [Acesse o Caderno aqui](https://notebook.google.com/notebook/be36bd28-0743-44c6-94cf-611c66340b85)

---

##  1. Visão Geral do Projeto
Este projeto tem como objetivo explorar o uso do **NotebookLM** como uma ferramenta de aprendizagem ativa e estruturação de conhecimento, aplicada ao estudo do **Mercado Financeiro e Educação Financeira**. 

A partir de uma curadoria de 5 documentos oficiais e regulatórios do setor financeiro brasileiro, a IA foi utilizada como um assistente técnico de estudos para extrair conceitos estratégicos, esclarecer estruturas de custos e riscos e sistematizar boas práticas de gestão orçamentária.

---

##  2. Curadoria de Fontes Utilizadas
O caderno temático no NotebookLM foi alimentado exclusivamente com as seguintes fontes oficiais:
1. **Caderno CVM 15 (Day Trade):** Análise do funcionamento, custos operacionais, riscos de alavancagem e vieses comportamentais.
2. **Caderno CVM 14 (BDR - Brazilian Depositary Receipts):** Estrutura de lastro, custódia, tipos de programas (Patrocinados e Não Patrocinados) e riscos cambiais/legais.
3. **Caderno CVM 13 (MRP - Mecanismo de Ressarcimento de Prejuízos):** Hipóteses de cobertura de até R$ 120.000,00 por danos causados por intermediários e o processo de acionamento.
4. **Regulamento do Tesouro Direto:** Regras gerais, papéis da STN, B3 e Agentes de Custódia, além dos direitos e deveres dos investidores.
5. **Caderno de Educação Financeira (Banco Central do Brasil):** Diretrizes para orçamento pessoal, Custo Efetivo Total (CET), uso do crédito e gestão de riscos.

---

##  3. Engenharia de Prompts e Resultados Sintetizados

###  Prompt 1: Análise de Riscos e Vieses no Day Trade
* **Prompt Utilizado:** *"Atue como um professor de finanças. Com base exclusivamente no Caderno CVM 15, explique o que é o Day Trade, quais são os principais custos e riscos dessa prática e quais vieses comportamentais costumam afetar esses investidores?"*
* **Principais Aprendizados Obtidos:**
  * **Conceito & Custos:** Operação realizada e liquidada no mesmo dia. Envolve custos de Corretagem, Custódia, Emolumentos da B3 e Imposto de Renda de 20% sobre o lucro líquido (sendo 1% retido na fonte via "dedo-duro").
  * **Riscos Severos:** A alavancagem pode gerar prejuízos superiores ao capital depositado. Dados da FGV/CVM mostram que mais de 92% dos praticantes desistem em menos de 300 pregões, sem evidências de curva de aprendizado acumulado.
  * **Vieses Comportamentais:** A tomada de decisão rápida expõe o trader a vieses como *Excesso de Confiança*, *Aversão à Perda* (dificuldade em estopar posições perdedoras), *Viés de Autocontrole* (tentar recuperar perdas impulsivamente) e *Efeito Manada*.

---

###  Prompt 2: Funcionamento e Riscos dos BDRs
* **Prompt Utilizado:** *"Com base no Caderno CVM 14, explique o que são BDRs (Brazilian Depositary Receipts), como eles funcionam, quais são os tipos/programas existentes e quais os principais riscos associados a esse investimento?"*
* **Principais Aprendizados Obtidos:**
  * **Mecanismo:** Certificados negociados na B3 em Reais que representam ativos emitidos no exterior (ações, títulos de dívida ou ETFs) mantidos sob custódia.
  * **Programas:** Divididos em *Patrocinados* (Níveis I, II e III, com participação da empresa emissora) e *Não Patrocinados* (Nível I, emitidos por instituições depositárias sem acordo direto com a empresa).
  * **Fatores de Risco:** Risco Cambial (mesmo que a ação externa suba, a valorização do Real frente ao Dólar pode reduzir o valor do BDR), Risco de Liquidez na B3 e diferenças nos padrões contábeis (ex: US GAAP vs. IFRS).

---

###  Prompt 3: Proteção ao Investidor com o MRP
* **Prompt Utilizado:** *"Utilizando o Caderno CVM 13, descreva o que é o Mecanismo de Ressarcimento de Prejuízos (MRP), em quais situações específicas o investidor pode solicitar esse ressarcimento e como funciona o processo para acioná-lo?"*
* **Principais Aprendizados Obtidos:**
  * **Escopo e Limite:** Instrumento mantido pela B3 que garante até **R$ 120.000,00** por ocorrência para prejuízos causados por erros/omissões de corretoras ou seus prepostos. *Não cobre oscilações normais do mercado nem produtos de balcão ou Tesouro Direto*.
  * **Hipóteses de Cobertura:** Operações não autorizadas, falhas técnicas comprovadas no Home Broker (sem alternativa da mesa), inexecução de ordens, *churning* (giro excessivo da carteira para gerar corretagem) e liquidação extrajudicial da corretora.
  * **Fluxo:** Solicitação via plataforma MRP Digital (BSM Supervisão de Mercados) em até 18 meses do fato, cabendo recurso administrativo ao Colegiado da CVM em caso de indeferimento.

---

###  Prompt 4: Normativa do Tesouro Direto
* **Prompt Utilizado:** *"Com base no Regulamento do Tesouro Direto, quais são as regras gerais de funcionamento do programa, os papéis das partes envolvidas (STN, B3, Agentes de Custódia e Investidores) e os principais direitos e deveres do investidor?"*
* **Principais Aprendizados Obtidos:**
  * **Operacionalização:** Parceria entre a Secretaria do Tesouro Nacional (STN - emissora) e a B3 (operadora dos sistemas e guardiã das contas de custódia).
  * **Agentes de Custódia:** Instituições intermediárias responsáveis pelo cadastro do investidor, recolhimento de impostos e execução financeira.
  * **Direitos e Deveres:** O investidor tem direito a contas individualizadas em seu nome e acesso direto aos saldos na B3. Tem o dever de manter o saldo disponível para liquidação (sob pena de suspensão temporária em caso de inadimplência) e custear as taxas regulamentares.

---

###  Prompt 5: Guia Prático de Educação Financeira (Banco Central)
* **Prompt Utilizado:** *"Com base no Caderno de Educação Financeira do Banco Central, crie um guia prático de organização financeira cobrindo: orçamento pessoal, uso consciente do crédito, consumo planejado e prevenção de riscos financeiros."*
* **Principais Aprendizados Obtidos:**
  * **Orçamento:** Estruturado em 4 etapas (Planejamento, Registro, Agrupamento e Avaliação) com foco no saldo superavitário e na regra do *"Pague-se Primeiro"*.
  * **Crédito Consciente:** Necessidade de avaliar sempre o **CET (Custo Efetivo Total)** e não apenas os juros nominais. Estratégias claras para renegociação de dívidas e portabilidade.
  * **Prevenção de Riscos:** Constituição de Reserva de Emergência de alta liquidez e baixo risco antes de investimentos mais arriscados, aliada à contratação consciente de seguros e proteção digital.

---

##  4. Documentação de Aprendizado e Desafios (Feedback da IA)

### O que funcionou bem:
* **Fidelidade às Fontes:** O uso do NotebookLM impediu a ocorrência de alucinações. Todas as respostas contiveram dados precisos embasados estritamente nos regulamentos da CVM, STN e Banco Central.
* **Capacidade de Síntese:** A IA estruturou com clareza a diferença entre os níveis de BDRs e organizou os vieses comportamentais em uma lista didática de rápido consumo.

### Dificuldades Encontradas e Ajustes de Prompt:
* **Delimitação de Escopo:** Para evitar que o modelo misturasse o funcionamento de garantias, foi necessário explicitar no Prompt 3 que o MRP **não cobre títulos do Tesouro Direto nem renda fixa de balcão**, apenas operações de bolsa.
* **Engenharia de Persona:** A definição clara do papel no prompt (*"Atue como um professor de finanças"*) ajudou o modelo a adotar uma linguagem explicativa, evitando o tom meramente técnico/jurídico presente nos textos originais das resoluções.

---

## 5. Conclusão
O exercício demonstrou que o NotebookLM atua como uma ferramenta poderosa para potencializar a aprendizagem. A combinação de **curadoria rigorosa de fontes** com **engenharia de prompts direcionada** permitiu transformar mais de centenas de páginas de regulamentos financeiros complexos em um material didático, confiável e pronto para aplicação no dia a dia.
