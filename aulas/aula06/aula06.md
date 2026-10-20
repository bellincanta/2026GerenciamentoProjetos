# Aula 06 — Orçamento e Custeio de Projetos

## 1. Por que falar de custos?

Todo projeto vive dentro da chamada **restrição tripla**: escopo, prazo e custo. Mexer em um deles quase sempre afeta os outros. Em projetos de software, os estouros de orçamento normalmente nascem de:

- escopo mal definido (requisitos que "aparecem" no meio do caminho);
- estimativas otimistas ("isso é só uma telinha");
- riscos ignorados (API de terceiros instável, rotatividade da equipe);
- falta de acompanhamento — o problema só é percebido quando o dinheiro já acabou.

> **Ideia central:** orçamento não é um número que se "chuta" no início. É o resultado de um processo que parte do escopo (EAP), passa pelo cronograma e considera os riscos.

---

## 2. Os processos de gerenciamento de custos

Segundo o Guia PMBOK® (6ª edição), a área de **Gerenciamento dos Custos do Projeto** tem quatro processos:

| Processo | Pergunta que responde | Saída principal |
|---|---|---|
| **Planejar o gerenciamento dos custos** | Como vamos estimar, orçar e controlar? | Plano de gerenciamento dos custos |
| **Estimar os custos** | Quanto custa cada parte do trabalho? | Estimativas de custos + base das estimativas |
| **Determinar o orçamento** | Quanto o projeto custa no total e quando gastaremos? | Linha de base dos custos + requisitos de recursos financeiros |
| **Controlar os custos** | Estamos gastando conforme o planejado? | Medições de desempenho, previsões, solicitações de mudança |

> Na 7ª edição do PMBOK, o guia passou a ser organizado por **domínios de desempenho** (o custo aparece principalmente nos domínios de *Planejamento* e *Medição*). As técnicas, porém, continuam as mesmas — e são cobradas em certificações e no mercado.

---

## 3. Classificação dos custos

### 3.1 Diretos × Indiretos

- **Custos diretos:** atribuídos exclusivamente ao projeto.
  *Ex.: horas dos desenvolvedores alocados, servidor em nuvem contratado para o sistema, conta de publicação na loja de aplicativos.*
- **Custos indiretos:** compartilhados entre vários projetos e rateados.
  *Ex.: aluguel do escritório, energia elétrica, salário do setor administrativo, licença corporativa de ferramentas.*

### 3.2 Fixos × Variáveis

- **Fixos:** não mudam com o volume de trabalho. *Ex.: licença anual de uma IDE.*
- **Variáveis:** crescem conforme o trabalho. *Ex.: horas de programação, custo de nuvem por requisição.*

### 3.3 Outros conceitos úteis

- **Custo afundado (sunk cost):** dinheiro já gasto que não pode ser recuperado. **Não deve** influenciar a decisão de continuar ou não um projeto.
- **Custo de oportunidade:** o que se deixa de ganhar ao escolher uma alternativa em vez de outra.
- **Custo do ciclo de vida:** inclui não só o desenvolvimento, mas também operação e manutenção. Em software, a manutenção costuma superar o custo de desenvolvimento ao longo dos anos.

---

## 4. Técnicas de estimativa de custos

### 4.1 Estimativa análoga (top-down)

Usa um projeto **anterior semelhante** como referência.

> "O app de agendamento que fizemos no ano passado custou R$ 70 mil. Este é parecido, então deve custar algo próximo."

- ✅ Rápida e barata; útil no início, quando há pouca informação.
- ❌ Pouco precisa; depende de os projetos serem realmente parecidos.

### 4.2 Estimativa paramétrica

Usa uma **relação estatística** entre uma variável e o custo.

> Se a empresa sabe, pelo histórico, que cada **Ponto de Função** custa em média R$ 500, um sistema de 120 PF custará aproximadamente:
> **120 PF × R$ 500 = R$ 60.000**

- ✅ Pode ser bastante precisa se o histórico for bom.
- ❌ Exige dados históricos confiáveis e um modelo calibrado.

### 4.3 Estimativa bottom-up (de baixo para cima)

Estima-se o custo de **cada pacote de trabalho da EAP** e depois se soma tudo.

- ✅ A mais precisa.
- ❌ A mais trabalhosa; exige escopo bem detalhado.

### 4.4 Estimativa de três pontos

Considera a incerteza usando três valores:

- **O** — otimista (tudo dá certo)
- **M** — mais provável
- **P** — pessimista (os riscos se concretizam)

| Distribuição | Fórmula |
|---|---|
| Triangular (média simples) | E = (O + M + P) / 3 |
| Beta / **PERT** (mais usada) | **E = (O + 4M + P) / 6** |
| Desvio-padrão (PERT) | σ = (P − O) / 6 |

**Exemplo:** desenvolvimento do back-end
O = 160 h · M = 200 h · P = 300 h

- PERT: (160 + 4×200 + 300) / 6 = 1.260 / 6 = **210 h**
- Triangular: (160 + 200 + 300) / 3 = **220 h**
- σ = (300 − 160) / 6 ≈ **23,3 h**

> Observe que o resultado (210 h) é **maior** que o valor "mais provável" (200 h). Isso acontece porque o cenário pessimista está mais distante do provável do que o otimista — algo muito comum em software.

### 4.5 Precisão das estimativas

As estimativas vão ficando mais precisas conforme o projeto avança (*cone da incerteza*):

| Momento | Tipo | Faixa típica |
|---|---|---|
| Iniciação | Ordem de grandeza (ROM) | −25% a +75% |
| Planejamento | Orçamentária | −10% a +25% |
| Planejamento detalhado | Definitiva | −5% a +10% |

---

## 5. Do custo dos pacotes ao orçamento

### 5.1 A "pirâmide" do orçamento

```
┌─────────────────────────────────────────────┐
│               ORÇAMENTO DO PROJETO           │
│  ┌───────────────────────────────────────┐  │
│  │   Reserva gerencial  (fora da linha    │  │
│  │   de base — riscos desconhecidos)      │  │
│  ├───────────────────────────────────────┤  │
│  │        LINHA DE BASE DOS CUSTOS        │  │
│  │  ┌─────────────────────────────────┐  │  │
│  │  │ Reserva de contingência          │  │  │
│  │  │ (riscos identificados)           │  │  │
│  │  ├─────────────────────────────────┤  │  │
│  │  │ Estimativas dos pacotes de       │  │  │
│  │  │ trabalho (diretos + indiretos)   │  │  │
│  │  └─────────────────────────────────┘  │  │
│  └───────────────────────────────────────┘  │
└─────────────────────────────────────────────┘
```

- **Reserva de contingência:** para os riscos **conhecidos** ("sabemos que podem acontecer"). Faz parte da **linha de base** e o gerente do projeto pode utilizá-la.
- **Reserva gerencial:** para riscos **desconhecidos** ("o que não sabemos que não sabemos"). **Não** faz parte da linha de base; seu uso exige autorização do patrocinador/gerência.

### 5.2 Exemplo completo — App mobile de agendamento

**Passo 1 — Custo de mão de obra por pacote de trabalho (bottom-up)**

| EAP | Pacote de trabalho | Recurso | Horas | R$/h | Custo |
|---|---|---|---:|---:|---:|
| 1.1 | Levantamento de requisitos | Analista | 80 | 70,00 | 5.600,00 |
| 1.2 | Design UI/UX | Designer | 60 | 65,00 | 3.900,00 |
| 1.3 | Back-end (API) | Desenvolvedor | 200 | 75,00 | 15.000,00 |
| 1.4 | App React Native | Desenvolvedor | 240 | 75,00 | 18.000,00 |
| 1.5 | Testes | Testador | 100 | 55,00 | 5.500,00 |
| 1.6 | Implantação e publicação | Desenvolvedor | 40 | 75,00 | 3.000,00 |
| | **Subtotal mão de obra** | | **720** | | **51.000,00** |

**Passo 2 — Outros custos diretos**

| Item | Cálculo | Custo |
|---|---|---:|
| Servidor em nuvem | 6 meses × R$ 400 | 2.400,00 |
| Contas de desenvolvedor nas lojas | — | 700,00 |
| Dispositivos para testes | — | 2.900,00 |
| **Subtotal** | | **6.000,00** |

**Passo 3 — Custos indiretos**
Política da empresa: rateio de **10%** sobre os custos diretos.
(51.000 + 6.000) × 10% = **R$ 5.700,00**

**Estimativa total dos pacotes:** 57.000 + 5.700 = **R$ 62.700,00**

**Passo 4 — Reserva de contingência (a partir da análise de riscos)**

Valor Monetário Esperado (VME) = probabilidade × impacto

| Risco identificado | Prob. | Impacto | VME |
|---|---:|---:|---:|
| API de pagamento de terceiros mudar | 30% | R$ 8.000 | 2.400,00 |
| Saída de um desenvolvedor | 20% | R$ 10.000 | 2.000,00 |
| Reprovação na loja de apps | 10% | R$ 9.000 | 900,00 |
| **Total** | | | **5.300,00** |

**Linha de base dos custos:** 62.700 + 5.300 = **R$ 68.000,00**

**Passo 5 — Reserva gerencial**
Política: 5% da linha de base → 68.000 × 5% = **R$ 3.400,00**

**Orçamento do projeto:** 68.000 + 3.400 = **R$ 71.400,00**

### 5.3 Distribuição no tempo — a Curva S

A linha de base não é só um valor total: ela é **distribuída ao longo do cronograma**. O gráfico do custo acumulado tem formato de "S" — gasta-se pouco no início, muito no meio (desenvolvimento) e pouco no fim.

| Mês | Atividades principais | Gasto no mês (R$) | Acumulado (R$) |
|---|---|---:|---:|
| 1 | Requisitos, design | 8.000 | 8.000 |
| 2 | Design, início back-end | 11.000 | 19.000 |
| 3 | Back-end, app | 16.000 | 35.000 |
| 4 | Back-end, app | 16.000 | 51.000 |
| 5 | App, testes | 11.000 | 62.000 |
| 6 | Testes, implantação | 6.000 | 68.000 |

```
R$ (mil)
 70 |                                   ●  68
 60 |                             ●  62
 50 |                       ●  51
 40 |
 30 |                 ●  35
 20 |           ●  19
 10 |     ●  8
  0 +-----+-----+-----+-----+-----+-----+
          1     2     3     4     5     6   mês
```

> Essa curva é o **Valor Planejado (VP)** acumulado — a referência que usaremos no controle de custos.

---

## 6. Controle de custos — Gerenciamento do Valor Agregado (EVM)

Saber apenas que "gastamos R$ 40 mil até agora" **não diz nada** se não soubermos quanto trabalho foi entregue. O EVM cruza **três medidas**:

| Sigla (PT) | Sigla (EN) | Nome | Significado |
|---|---|---|---|
| **VP** | PV | Valor Planejado | Quanto **deveríamos ter feito** até a data (em R$) |
| **VA** | EV | Valor Agregado | Quanto **realmente fizemos** (em R$ do orçamento) |
| **CR** | AC | Custo Real | Quanto **realmente gastamos** |
| **ONT** | BAC | Orçamento no Término | Orçamento total (linha de base) |

> **Como calcular o VA:** VA = % concluído × ONT (ou soma do valor orçado dos pacotes concluídos).

### 6.1 Variações e índices

| Indicador | Fórmula | Interpretação |
|---|---|---|
| **VC** — Variação de custo | VA − CR | < 0 → acima do orçamento |
| **VPr** — Variação de prazo | VA − VP | < 0 → atrasado |
| **IDC** — Índice de desempenho de custo | VA / CR | < 1 → cada R$ 1 gasto gera menos de R$ 1 de trabalho |
| **IDP** — Índice de desempenho de prazo | VA / VP | < 1 → progresso mais lento que o planejado |

> **Macete:** o VA vem **sempre primeiro**. E, nos índices, **acima de 1 é bom, abaixo de 1 é ruim**.

### 6.2 Previsões

| Indicador | Fórmula | Quando usar |
|---|---|---|
| **ENT** — Estimativa no término (típica) | ONT / IDC | O desempenho atual vai continuar |
| **ENT** (atípica) | CR + (ONT − VA) | O desvio foi pontual e não se repetirá |
| **ENT** (custo e prazo) | CR + (ONT − VA) / (IDC × IDP) | Custo e atraso influenciarão o restante |
| **EPT** — Estimativa para terminar | ENT − CR | Quanto ainda falta gastar |
| **VNT** — Variação no término | ONT − ENT | Quanto vamos estourar (ou economizar) |
| **IDPT** — Índice de desempenho para término | (ONT − VA) / (ONT − CR) | Eficiência necessária daqui pra frente |

### 6.3 Exemplo resolvido

Projeto de R$ 100.000 (ONT), duração de 10 meses, distribuição linear.
No **fim do mês 5**:

- Planejado: 50% → **VP = R$ 50.000**
- Concluído: 40% → **VA = R$ 40.000**
- Gasto: **CR = R$ 48.000**

| Indicador | Cálculo | Resultado | Leitura |
|---|---|---:|---|
| VC | 40.000 − 48.000 | **−8.000** | Acima do orçamento |
| VPr | 40.000 − 50.000 | **−10.000** | Atrasado |
| IDC | 40.000 / 48.000 | **0,83** | Cada R$ 1,00 gera R$ 0,83 de trabalho |
| IDP | 40.000 / 50.000 | **0,80** | Avançando a 80% do ritmo planejado |
| ENT (típica) | 100.000 / 0,8333 | **120.000** | Deve terminar custando R$ 120 mil |
| EPT | 120.000 − 48.000 | **72.000** | Ainda faltam R$ 72 mil |
| VNT | 100.000 − 120.000 | **−20.000** | Estouro previsto de R$ 20 mil |
| IDPT | 60.000 / 52.000 | **1,15** | Precisaria ser 15% mais eficiente para fechar no orçamento |

Comparando os cenários de previsão:

- **Atípica:** 48.000 + 60.000 = R$ 108.000
- **Típica:** R$ 120.000
- **Custo e prazo:** 48.000 + 60.000 / (0,8333 × 0,8) = 48.000 + 90.000 = R$ 138.000

> **Diagnóstico:** o projeto está **atrasado e acima do orçamento**. Um IDPT de 1,15 é muito difícil de alcançar — o gerente deve levar ao patrocinador uma solicitação de mudança (aumento de orçamento, redução de escopo ou ambos).

### 6.4 Quadro de diagnóstico rápido

| | **IDP ≥ 1** (no prazo/adiantado) | **IDP < 1** (atrasado) |
|---|---|---|
| **IDC ≥ 1** (dentro do orçamento) | 🟢 Situação ideal | 🟡 Economizando, mas lento — falta gente? |
| **IDC < 1** (acima do orçamento) | 🟡 Rápido, mas caro — horas extras? | 🔴 Situação crítica |

---

## 7. Custos em projetos ágeis

Em times ágeis (Scrum), o raciocínio muda um pouco: a equipe e a duração da sprint são fixas, então o **custo por sprint** é praticamente constante.

> Time de 5 pessoas × 80 h por sprint × R$ 70/h ≈ **R$ 28.000 por sprint**

Se o backlog tem 300 *story points* e a **velocidade** média do time é 30 pontos/sprint:
300 / 30 = 10 sprints → **10 × R$ 28.000 = R$ 280.000**

Aqui, o que costuma variar é o **escopo** (o que cabe nas sprints), e não o custo. Existe ainda uma adaptação do EVM para ágil (*AgileEVM*), que usa pontos entregues no lugar do percentual concluído.

---

## 8. Resumo

- O orçamento nasce da **EAP**: estima-se cada pacote, soma-se, adicionam-se as reservas.
- **Linha de base** = estimativas + reserva de contingência.
- **Orçamento** = linha de base + reserva gerencial.
- O controle é feito com o **EVM**: VP, VA e CR → VC, VPr, IDC, IDP → previsões (ENT, EPT, VNT).
- **IDC e IDP abaixo de 1** são sinais de alerta e precisam virar ação.

---

## 9. Exercícios

**Exercício 1 — Três pontos.**
A equipe estimou a tela de cadastro com O = 20 h, M = 30 h e P = 52 h. Calcule a estimativa PERT e o desvio-padrão. Se a hora custa R$ 80, qual o custo estimado?

**Exercício 2 — Classificação.**
Classifique cada custo como **direto ou indireto** e **fixo ou variável**:
a) Horas do desenvolvedor alocado só neste projeto
b) Aluguel do escritório da empresa
c) Licença anual do Figma comprada para este projeto
d) Custo de nuvem cobrado por número de acessos

**Exercício 3 — Orçamento.**
As estimativas dos pacotes somam R$ 80.000. A análise de riscos resultou em R$ 6.000 de contingência, e a gerência definiu R$ 4.300 de reserva gerencial. Determine a linha de base e o orçamento total.

**Exercício 4 — Valor agregado.**
Um projeto com ONT = R$ 200.000 apresenta, na data de status: VP = R$ 120.000, VA = R$ 100.000 e CR = R$ 125.000.
a) Calcule VC, VPr, IDC e IDP.
b) Calcule ENT (típica), EPT e VNT.
c) Escreva um parágrafo diagnosticando a situação para o patrocinador.

**Exercício 5 — Discursivo.**
Por que a reserva gerencial **não** faz parte da linha de base dos custos? O que aconteceria com os indicadores do EVM se ela fosse incluída?

**Exercício 6 — Prática em grupo.**
Usando a EAP do projeto da equipe (trabalho da disciplina), monte uma planilha bottom-up com: pacotes de trabalho, recurso, horas, valor/hora, outros custos diretos, indiretos (10%), reserva de contingência (com ao menos 3 riscos) e reserva gerencial. Apresente também a distribuição mensal (Curva S).

---

## Referências

- PROJECT MANAGEMENT INSTITUTE. **Um guia do conhecimento em gerenciamento de projetos (Guia PMBOK®)**. 6. ed. Newtown Square: PMI, 2017. Cap. 7.
- PROJECT MANAGEMENT INSTITUTE. **Guia PMBOK®**. 7. ed. Newtown Square: PMI, 2021.
- VARGAS, Ricardo. **Gerenciamento de projetos: estabelecendo diferenciais competitivos**. Rio de Janeiro: Brasport.
- VARGAS, Ricardo. **Análise de valor agregado em projetos**. Rio de Janeiro: Brasport.
- SOMMERVILLE, Ian. **Engenharia de software**. São Paulo: Pearson. (capítulo sobre planejamento e estimativa de projetos)

---
---

## 📌 Notas do professor

### Plano sugerido

| Tempo | Encontro 1 | Encontro 2 |
|---|---|---|
| 0–15 min | Problematização: "quanto custa um app?" (deixar a turma chutar e anotar no quadro) | Revisão rápida: linha de base × orçamento |
| 15–50 min | Seções 2, 3 e 4 (classificação e técnicas) | Seção 6 (EVM) com o exemplo resolvido |
| 50–80 min | Seção 5 — construir o exemplo do app **junto** com a turma | Exercícios 4 e 5 em duplas |
| 80–100 min | Exercícios 1, 2 e 3 | Início do exercício 6 (projeto da equipe) |

**Dica:** no início do encontro 1, guarde os "chutes" da turma. Ao final da seção 5, compare com o R$ 71.400 calculado — costuma gerar uma boa discussão sobre por que estimativas intuitivas são quase sempre otimistas.

**Pontos de atenção comuns:**
- Alunos confundem **VA** (valor agregado) com **CR** (custo real). Reforçar: VA é medido em R$ *do orçamento*, não em R$ gastos.
- Muitos incluem a reserva gerencial na linha de base. Retomar a figura da seção 5.1.
- Na estimativa PERT, alguns esquecem o peso 4 no valor mais provável.

### Gabarito

**Exercício 1**
- PERT: (20 + 4×30 + 52) / 6 = 192 / 6 = **32 h**
- σ = (52 − 20) / 6 ≈ **5,33 h**
- Custo: 32 × 80 = **R$ 2.560,00**

**Exercício 2**
a) Direto, variável
b) Indireto, fixo
c) Direto, fixo
d) Direto, variável

**Exercício 3**
- Linha de base: 80.000 + 6.000 = **R$ 86.000**
- Orçamento: 86.000 + 4.300 = **R$ 90.300**

**Exercício 4**
a) VC = 100.000 − 125.000 = **−25.000** · VPr = 100.000 − 120.000 = **−20.000** · IDC = 100.000 / 125.000 = **0,80** · IDP = 100.000 / 120.000 ≈ **0,83**
b) ENT = 200.000 / 0,80 = **R$ 250.000** · EPT = 250.000 − 125.000 = **R$ 125.000** · VNT = 200.000 − 250.000 = **−R$ 50.000**
c) Espera-se que o aluno diga que o projeto está **atrasado e acima do orçamento** (quadrante vermelho), que, mantido o desempenho, custará R$ 50 mil a mais (25% acima) e que é necessária uma ação: análise de causa, replanejamento, solicitação de mudança (orçamento/escopo/prazo). Valorizar textos claros e sem jargão excessivo — o leitor é o patrocinador.

**Exercício 5 (resposta esperada)**
A reserva gerencial cobre riscos **desconhecidos** e é controlada pela gerência/patrocinador, não pelo gerente do projeto. Como não está associada a nenhuma atividade planejada, não pode ser distribuída no cronograma. Se fosse incluída na linha de base, o ONT e o VP ficariam inflados, mascarando o desempenho: o IDC pareceria melhor do que é e as previsões (ENT, VNT) perderiam a utilidade como sinal de alerta.

### Rubrica — Exercício 6 (A/B/C/D)

| Critério | A | B | C | D |
|---|---|---|---|---|
| **Estimativa bottom-up** | Todos os pacotes da EAP com recurso, horas e valor/hora coerentes | Quase todos os pacotes; pequenas incoerências | Pacotes agrupados ou valores sem justificativa | Valor global "chutado", sem relação com a EAP |
| **Reservas** | Contingência calculada por VME (≥ 3 riscos) e gerencial separada corretamente | Contingência por VME, mas com riscos genéricos | Reservas como percentual fixo sem justificativa | Reservas ausentes ou misturadas |
| **Linha de base × orçamento** | Distinção correta e explicada | Distinção correta, sem explicação | Valores corretos com nomenclatura trocada | Conceitos confundidos |
| **Curva S** | Distribuição mensal coerente com o cronograma | Distribuição coerente, com pequenos desvios | Distribuição linear sem relação com as atividades | Ausente |

**Feedback sugerido por conceito:**
- **A:** "O orçamento de vocês nasce da EAP e considera os riscos de forma mensurável — é exatamente o que se espera de um planejamento profissional."
- **B:** "A estrutura está correta. Detalhem melhor os riscos e as horas de cada pacote para deixar a estimativa mais defensável."
- **C:** "Os números aparecem, mas falta a ligação com a EAP e com a análise de riscos. Revisem a seção 5.2 e refaçam a partir dos pacotes de trabalho."
- **D:** "O orçamento ainda não foi construído a partir do escopo. Vamos conversar em atendimento para refazer o passo a passo."
