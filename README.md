# Desafio DIO: Treinando uma IA de Aprendizagem com o NotebookLM

> **Link de acesso ao Caderno no NotebookLM:** [Acesse o Caderno aqui](https://notebook.google.com/notebook/be36bd28-0743-44c6-94cf-611c66340b85)

---

## 1. Contexto e Objetivos de Estudo

Este projeto explora o uso do NotebookLM como uma ferramenta de aprendizagem ativa e gestão do conhecimento aplicados à Educação Financeira e Mercado Financeiro.

### Objetivos de Estudo:
* Compreender o funcionamento de produtos financeiros como BDRs e títulos do Tesouro Direto.
* Mapear os riscos operacionais, tributação e vieses comportamentais envolvidos no Day Trade.
* Entender a cobertura e o processo de acionamento do Mecanismo de Ressarcimento de Prejuízos (MRP).
* Estruturar um guia de organização financeira pessoal com foco em orçamento, uso consciente do crédito e prevenção de riscos.

---

## 2. Curadoria de Fontes Utilizadas

O caderno temático no NotebookLM foi alimentado com 5 documentos oficiais e regulatórios do setor financeiro brasileiro:

1. **Caderno CVM 15 (Day Trade):** Análise de funcionamento, custos operacionais, riscos de alavancagem e vieses comportamentais.
2. **Caderno CVM 14 (BDR - Brazilian Depositary Receipts):** Lastro, custódia, programas patrocinados/não patrocinados e riscos cambiais/legais.
3. **Caderno CVM 13 (MRP - Mecanismo de Ressarcimento de Prejuízos):** Hipóteses de cobertura (até R$ 120.000,00) por danos de intermediários e fluxo de acionamento.
4. **Regulamento do Tesouro Direto:** Regras gerais, papéis da STN, B3 e Agentes de Custódia, direitos e deveres do investidor.
5. **Caderno de Educação Financeira (Banco Central do Brasil):** Orçamento pessoal, Custo Efetivo Total (CET), uso de crédito e gestão de riscos.

---

## 3. Engenharia de Prompts e Troubleshooting

### Prompt 1: Análise de Riscos e Vieses no Day Trade
* **Prompt Utilizado:** *"Atue como um professor de finanças. Com base exclusivamente no Caderno CVM 15, explique o que é o Day Trade, quais são os principais custos e riscos dessa prática e quais vieses comportamentais costumam afetar esses investidores?"*
* **Resultado e Referências:** Detalhou corretagem, emolumentos, IR de 20% (1% na fonte via dedo-duro), alavancagem e apontou que mais de 92% dos praticantes desistem em menos de 300 pregões. Mapeou vieses como Aversão à Perda, Excesso de Confiança e Efeito Manada.

---

### Prompt 2: Funcionamento e Riscos dos BDRs
* **Prompt Utilizado:** *"Com base no Caderno CVM 14, explique o que são BDRs (Brazilian Depositary Receipts), como eles funcionam, quais são os tipos/programas existentes e quais os principais riscos associados a esse investimento?"*
* **Resultado e Referências:** Explicou a relação de lastro mantida por instituição depositária, a diferença entre programas Patrocinados (Níveis I, II e III) e Não Patrocinados, além dos riscos cambial, de liquidez e divergências contábeis.

---

### Prompt 3: Proteção ao Investidor com o MRP
* **Prompt Utilizado:** *"Utilizando o Caderno CVM 13, descreva o que é o Mecanismo de Ressarcimento de Prejuízos (MRP), em quais situações específicas o investidor pode solicitar esse ressarcimento e como funciona o processo para acioná-lo?"*
* **Resultado e Referências:** Mapeou o limite de cobertura de R$ 120.000,00 por evento e as hipóteses (ordens não autorizadas, falhas de Home Broker, churning e liquidação da corretora).

---

### Prompt 4: Normativa do Tesouro Direto
* **Prompt Utilizado:** *"Com base no Regulamento do Tesouro Direto, quais são as regras gerais de funcionamento do programa, os papéis das partes envolvidas (STN, B3, Agentes de Custódia e Investidores) e os principais direitos e deveres do investidor?"*
* **Resultado e Referências:** Detalhou os papéis da STN (emissora), B3 (operadora), Agentes de Custódia (intermediários) e os deveres do investidor (liquidação financeira dentro do prazo e manutenção de dados atualizados).

---

### Prompt 5: Guia Prático de Educação Financeira (Banco Central)
* **Prompt Utilizado:** *"Com base no Caderno de Educação Financeira do Banco Central, crie um guia prático de organização financeira cobrindo: orçamento pessoal, uso consciente do crédito, consumo planejado e prevenção de riscos financeiros."*
* **Resultado e Referências:** Estruturou o método de orçamento em 4 etapas (Planejamento, Registro, Agrupamento e Avaliação), destacou a regra do "Pague-se Primeiro" e a importância de analisar o CET em empréstimos.

---

### Dificuldades Encontradas e Ajustes (Troubleshooting):
* **Delimitação de Escopo:** Para evitar que o modelo misturasse o funcionamento de garantias, foi necessário explicitar no Prompt 3 que o MRP **não cobre títulos do Tesouro Direto nem renda fixa de balcão**, apenas operações de bolsa.
* **Engenharia de Persona:** A definição clara do papel no prompt (*"Atue como um professor de finanças"*) ajudou o modelo a adotar uma linguagem explicativa, evitando o tom meramente técnico/jurídico presente nos textos originais das resoluções.

---

## 4. Miniguia de Estudo (Entrega Final)

### Glossário de Conceitos Aprendidos
* **BDR (Brazilian Depositary Receipt):** Certificado de depósito negociado no Brasil que representa valores mobiliários emitidos por empresas ou ETFs no exterior.
* **CET (Custo Efetivo Total):** Taxa percentual que representa o custo total real de um empréstimo ou financiamento, somando juros, tarifas, tributos (IOF) e seguros.
* **Churning:** Prática ilegal de giro excessivo e injustificado da carteira do cliente por um intermediário financeiro para gerar comissões de corretagem.
* **Day Trade:** Operação de compra e venda (ou venda e compra) de um mesmo ativo realizada no mesmo dia pelo mesmo investidor.
* **MRP (Mecanismo de Ressarcimento de Prejuízos):** Garantia de até R$ 120.000,00 administrada pela BSM/B3 para ressarcir prejuízos causados por erros ou fraudes de corretoras.
* **STN (Secretaria do Tesouro Nacional):** Órgão do governo federal responsável pela emissão dos títulos públicos oferecidos no Tesouro Direto.
* **Viés da Aversão à Perda:** Tendência psicológica de sentir a dor da perda financeira de forma mais intensa que o prazer de um ganho equivalente, levando o investidor a manter posições perdedoras por tempo excessivo.

---

### Prompts Reutilizáveis para Revisões Futuras
Guarde estes prompts para usar quando precisar revisar o conteúdo do caderno:
1. **Revisão Rápida:** *"Crie um quiz de 5 perguntas de múltipla escolha com gabarito comentado sobre as diferenças entre BDR Patrocinado e Não Patrocinado baseando-se no Caderno CVM 14."*
2. **Resumo Executivo:** *"Elabore um checklist de 5 passos que o investidor deve seguir caso precise acionar o MRP (Mecanismo de Ressarcimento de Prejuízos) da B3."*
3. **Simulação Prática:** *"Atue como um consultor financeiro e me dê um exemplo prático comparando duas opções de empréstimo utilizando a análise do CET (Custo Efetivo Total) conforme orienta o Banco Central."*

---

## 5. Conclusão

O projeto demonstrou que o NotebookLM atua como um excelente copiloto de aprendizagem. A combinação de curadoria rigorosa de fontes com engenharia de prompts direcionada permitiu transformar documentos regulatórios complexos em um miniguia estruturado, didático e acionável.
