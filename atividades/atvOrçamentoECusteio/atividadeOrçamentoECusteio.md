# Atividade Avaliativa — Orçamento e Custeio: da aula ao seu projeto de TCC

**Instituto Federal do Paraná — Campus Cascavel**

**Curso Superior de Tecnologia em Análise e Desenvolvimento de Sistemas**

Disciplina: Gerenciamento de Projetos · Prof. Nelson Bellincanta Filho

| Item | Definição |
| --- | --- |
| **Modalidade** | Individual |
| **Entrega** | Artigo no modelo SBC, 2 a 4 páginas (PDF) |
| **Pré-requisito** | EAP do seu TCC (mesmo que preliminar) |

## 1. Texto-base

Material da disciplina: **Aula 06 — Orçamento e Custeio de Projetos** (processos de gerenciamento de custos, classificação de custos, técnicas de estimativa, reservas, Curva S e Gerenciamento do Valor Agregado — EVM).

Acessar o material da aula (aula06.md)

Leitura complementar: PROJECT MANAGEMENT INSTITUTE. **Guia PMBOK®**. 6. ed. Newtown Square: PMI, 2017. Cap. 7 — Gerenciamento dos Custos do Projeto.

## 2. Objetivos de aprendizagem

- Compreender por que o orçamento é o **resultado de um processo** (EAP → estimativas → riscos → reservas) e não um número estimado de forma intuitiva no início do projeto.
- Diferenciar custos diretos e indiretos, fixos e variáveis, e reconhecer conceitos como custo afundado e custo de oportunidade em um projeto real.
- Aplicar técnicas de estimativa (em especial bottom-up e três pontos/PERT) e distinguir **linha de base dos custos** de **orçamento do projeto**.
- **Transferir** os conceitos da aula para um projeto real e próprio — o seu TCC — construindo uma estimativa, um orçamento com reservas, uma Curva S e um diagnóstico por valor agregado, em vez de tratar o esforço do TCC como algo que "se resolve no fim".
- Produzir e justificar decisões de projeto documentadas, com base em números e critérios explícitos, e não em intuição.

## 3. Etapa 1 — Leitura dirigida do material

Estude o material da Aula 06 integralmente e responda, com suas próprias palavras (respostas curtas, de 3 a 6 linhas cada). Sempre que usar uma ideia do material, indique a seção ou a obra de referência (PMBOK, Vargas, Sommerville).

1. O material afirma que **o orçamento não é um número que se "chuta" no início**, mas o resultado de um processo que parte do escopo (EAP), passa pelo cronograma e considera os riscos. Relacione essa ideia com a **restrição tripla** (escopo, prazo e custo) e com as quatro causas típicas de estouro de orçamento em projetos de software citadas na seção 1.
2. O PMBOK 6ª edição organiza o Gerenciamento dos Custos em **quatro processos**. Cite-os, indique a pergunta que cada um responde e explique o que muda na 7ª edição, organizada por domínios de desempenho.
3. Explique a diferença entre custos **diretos e indiretos** e entre custos **fixos e variáveis**. Em seguida, explique por que o **custo afundado** não deve influenciar a decisão de continuar ou abandonar um projeto e dê um exemplo dessa armadilha em um projeto de software (ex.: insistir em uma tecnologia só porque já se investiu muito tempo nela).
4. Compare as estimativas **análoga, paramétrica, bottom-up e de três pontos** quanto à precisão, ao esforço e ao momento do projeto em que cada uma é mais adequada. Por que, no exemplo do back-end, a estimativa PERT (210 h) ficou **acima** do valor mais provável (200 h)? Relacione sua resposta ao **cone da incerteza**.
5. Explique a diferença entre **reserva de contingência** e **reserva gerencial**: que tipo de risco cada uma cobre, quem pode utilizá-la e por que apenas uma delas faz parte da **linha de base dos custos**.
6. O material afirma que saber apenas que "gastamos R$ 40 mil até agora" **não diz nada**. Por quê? Explique o papel de **VP, VA e CR** no Gerenciamento do Valor Agregado e interprete o que significa um projeto com **IDC = 0,83 e IDP = 0,80**, usando o quadro de diagnóstico rápido (seção 6.4).

## 4. Etapa 2 — Orçamento e controle de custos do seu TCC

Esta é a parte principal da atividade. Trate o seu TCC como um **projeto real**, com escopo (sua EAP), prazo (calendário do curso) e custo — e construa para ele um orçamento como o do exemplo do app de agendamento (seção 5.2 da aula).

> **Antes de começar: o principal custo do seu TCC é o seu tempo.** Ninguém está pagando suas horas, mas elas têm valor — é o **custo de oportunidade** (seção 3.3): cada hora no TCC é uma hora a menos de estágio, trabalho ou outra disciplina. Por isso, atribua um **valor/hora** às suas horas e **justifique** a escolha (ex.: salário de um desenvolvedor júnior na região, valor da sua bolsa ou estágio, tabela de referência de mercado). O orientador pode ser tratado como recurso com horas próprias ou como o **patrocinador** do projeto — deixe sua escolha explícita.

### 4.1 Caracterização do projeto

Apresente em meia página: tema e objetivo do TCC, entregas previstas (produto de software, artigo, apresentação), prazo final, duração em meses, recursos envolvidos (você, orientador, colegas de equipe, se houver) e o valor/hora adotado, com a justificativa.

### 4.2 Estimativa dos pacotes de trabalho (bottom-up com três pontos)

A partir da EAP do seu TCC, estime **no mínimo seis** pacotes de trabalho (ex.: revisão de literatura, requisitos, protótipo, back-end, front-end/app, testes, redação do artigo, preparação da defesa). Para cada pacote, informe as horas otimista (O), mais provável (M) e pessimista (P), calcule a estimativa PERT — E = (O + 4M + P) / 6 — e o desvio-padrão — σ = (P − O) / 6 — e o custo.

| EAP | Pacote de trabalho | Recurso | O (h) | M (h) | P (h) | PERT (h) | σ (h) | R$/h | Custo (R$) |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1.1 |  |  |  |  |  |  |  |  |  |
| 1.2 |  |  |  |  |  |  |  |  |  |
| 1.3 |  |  |  |  |  |  |  |  |  |
| 1.4 |  |  |  |  |  |  |  |  |  |
| 1.5 |  |  |  |  |  |  |  |  |  |
| 1.6 |  |  |  |  |  |  |  |  |  |
|  | **Total** |  |  |  |  |  |  |  |  |

*Quadro 1 — Estimativa bottom-up de três pontos dos pacotes de trabalho do TCC.*

### 4.3 Outros custos e classificação

Levante os demais custos do seu TCC e classifique cada um como **direto ou indireto** e **fixo ou variável**. Inclua, no mínimo, três custos diretos além da mão de obra (ex.: hospedagem ou nuvem, domínio, API paga, conta de desenvolvedor em loja de apps, dispositivo para testes, impressão e encadernação) e calcule os **custos indiretos** — internet, energia elétrica, depreciação do notebook — por rateio (use 10%, como na aula, ou justifique outro percentual).

| Item de custo | Direto/Indireto | Fixo/Variável | Cálculo | Custo (R$) |
| --- | --- | --- | --- | --- |
| 1. |  |  |  |  |
| 2. |  |  |  |  |
| 3. |  |  |  |  |
| 4. |  |  |  |  |
|  |  |  | **Total** |  |

*Quadro 2 — Outros custos do projeto de TCC e sua classificação.*

### 4.4 Reservas, linha de base e orçamento

Identifique **no mínimo três** riscos reais e específicos do seu TCC e calcule a **reserva de contingência** pelo Valor Monetário Esperado (VME = probabilidade × impacto). Expresse o impacto em R$ (horas de retrabalho × valor/hora, ou custo direto adicional). Em seguida, defina a **reserva gerencial** (ex.: 5% da linha de base) e apresente a composição final.

| Risco identificado | Probabilidade (%) | Impacto (R$) | VME (R$) |
| --- | --- | --- | --- |
| 1. |  |  |  |
| 2. |  |  |  |
| 3. |  |  |  |
| **Reserva de contingência** |  |  |  |

*Quadro 3 — Reserva de contingência do projeto de TCC.*

Apresente, logo abaixo do quadro, o cálculo explícito de: estimativa dos pacotes (Quadros 1 + 2) → **linha de base dos custos** (+ contingência) → **orçamento do projeto** (+ reserva gerencial).

**Exemplos de riscos com impacto em custo em TCC de TADS** (use como inspiração, não copie): API gratuita passar a ser paga; retrabalho após a banca de qualificação; perda de código sem backup; troca de tecnologia no meio do desenvolvimento; reprovação do app na loja; redução de horas disponíveis por causa de estágio ou trabalho.

### 4.5 Distribuição no tempo — Curva S

Distribua a linha de base ao longo dos meses do TCC, de acordo com o seu cronograma real (as atividades de cada mês), e apresente o gráfico do custo acumulado. A distribuição deve refletir as atividades — evite simplesmente dividir o total pelo número de meses.

| Mês | Atividades principais | Gasto no mês (R$) | Acumulado — VP (R$) |
| --- | --- | --- | --- |
| 1 |  |  |  |
| 2 |  |  |  |
| 3 |  |  |  |
| 4 |  |  |  |
| ... |  |  |  |

*Quadro 4 — Distribuição da linha de base (Curva S) do projeto de TCC.*

### 4.6 Cenário de controle — valor agregado

Escolha uma **data de status** no meio do seu cronograma e simule (ou, se o TCC já está em andamento, meça de verdade) a situação do projeto nesse ponto:

- Informe **VP** (do Quadro 4), **VA** (soma do valor orçado dos pacotes concluídos) e **CR** (horas realmente gastas × valor/hora + custos diretos já pagos).
- Calcule **VC, VPr, IDC, IDP, ENT (típica), EPT, VNT e IDPT**, mostrando os cálculos.
- Classifique o projeto no quadro de diagnóstico rápido (seção 6.4 da aula) e escreva um parágrafo de diagnóstico **dirigido ao seu orientador**, como se ele fosse o patrocinador: o que está acontecendo, por quê e qual ação você propõe (replanejamento, redução de escopo, uso da reserva de contingência ou solicitação de mudança no prazo).
- Para este cenário, qual fórmula de ENT (típica, atípica ou de custo e prazo) é mais realista no seu caso? Justifique.

### 4.7 Confronto com o material

Responda de forma honesta e argumentada:

- Antes desta atividade, você tinha alguma estimativa de quantas horas o seu TCC exigiria, ou o esforço era tratado de forma intuitiva ("vai dar tempo")? Compare sua estimativa intuitiva inicial com o total PERT do Quadro 1 e comente a diferença.
- O material afirma que estimativas intuitivas são quase sempre **otimistas**. Isso se confirmou no seu caso? Em quais pacotes a diferença entre O e P foi maior, e o que isso revela sobre a incerteza do seu projeto?
- Existe algum **custo afundado** no seu TCC hoje (tecnologia, tema ou abordagem que você mantém só porque já investiu tempo nela)? Como a leitura muda a sua decisão sobre ele?

## 5. Estrutura e formato do relatório

O relatório deve ser redigido **no formato de artigo científico, seguindo o modelo de publicações da SBC (Sociedade Brasileira de Computação)** — o mesmo template adotado nos TCCs do curso. Além do conteúdo, será avaliada a correta aplicação do modelo, pois esta atividade também serve de treino para a escrita do seu próprio TCC.

### 5.1 Padrão de formatação

- Artigo no modelo SBC (o mesmo do TCC), 2 a 4 páginas (PDF). Tabelas grandes (ex.: Tabela 1) podem usar fonte reduzida, desde que legíveis.
- Fórmulas usadas nos cálculos (PERT, VME, IDC, IDP, ENT) devem aparecer ao menos uma vez no texto.

### 5.2 Seções obrigatórias

- **1. Introdução** — tema e objetivo do seu TCC, contexto do problema e por que estimar, orçar e controlar custos é relevante nesse projeto, mesmo sem um cliente pagante. Encerre indicando o objetivo do relatório e como ele está organizado.
- **2. Referencial Teórico** — síntese crítica do material (Etapa 1), organizada em subseções, por exemplo: *2.1 Gerenciamento dos custos e restrição tripla*; *2.2 Classificação de custos*; *2.3 Técnicas de estimativa*; *2.4 Linha de base, reservas e orçamento*; *2.5 Gerenciamento do Valor Agregado*. Redija em texto corrido, com citações — não como lista de respostas às questões.
- **3. Material e Métodos** — como você construiu o orçamento: origem da EAP, como estimou as horas O, M e P (histórico próprio, opinião do orientador, comparação com TCCs anteriores), justificativa do valor/hora, critério de rateio dos indiretos, como estimou probabilidade e impacto dos riscos, e limitações da análise.
- **4. Resultados e Discussão** — a Etapa 2: a estimativa bottom-up (Quadro 1 reproduzido como **Tabela 1**), os demais custos (Quadro 2 como **Tabela 2**), as reservas e o orçamento (Quadro 3 como **Tabela 3**, com o cálculo da linha de base e do orçamento), a Curva S (Quadro 4 como **Tabela 4** e **Figura 1** com o gráfico acumulado), o cenário de valor agregado (item 4.6) e a discussão do item 4.7 confrontando sua prática com o que o material descreve.
- **5. Considerações Finais** — o que muda no planejamento e na condução do seu TCC a partir desta análise (prazos, escopo, reservas de tempo), e quais limitações permanecem.
- **Referências** — no padrão SBC (autor, ano, título, veículo), em ordem alfabética, incluindo obrigatoriamente o **Guia PMBOK® (PMI, 2017)** e ao menos uma das demais obras de referência da aula (Vargas — gerenciamento de projetos ou análise de valor agregado; Sommerville — Engenharia de Software).

---

> **Observação:** não existe resposta certa única nesta atividade. Um relatório que assume "eu imaginava umas 150 horas de TCC, a estimativa PERT deu 410, e com o meu estágio isso não cabe no calendário — vou precisar reduzir o escopo" vale mais do que um relatório com números redondos que "fecham" perfeitamente. Segundo o próprio material, estimativas que parecem confortáveis demais costumam ser apenas otimistas — e um orçamento sem reserva de contingência é sinal de riscos ignorados, não de um projeto sem riscos.
