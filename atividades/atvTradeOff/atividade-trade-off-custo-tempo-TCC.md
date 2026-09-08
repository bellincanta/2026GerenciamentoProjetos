# Atividade Avaliativa — Trade-off entre Custo e Tempo: do artigo científico ao seu projeto de TCC

**Instituto Federal do Paraná — Campus Cascavel**
**Curso Superior de Tecnologia em Análise e Desenvolvimento de Sistemas**

Disciplina: Gerenciamento de Projetos · Prof. Nelson Bellincanta Filho

| | |
|---|---|
| **Modalidade** | Individual |
| **Entrega** | Artigo no modelo SBC, 2 a 4 páginas (PDF) |

---

## 1. Texto-base

THIELMANN, Ricardo; QUEIROZ, Karen Oliveira Lopes de. **Trade-off entre custo e tempo em projetos.** *Revista Valore*, 2021. ISSN 2525-9008. DOI: [10.22408/reva602021629e-6007](https://doi.org/10.22408/reva602021629e-6007).

📄 **[Acessar o artigo (PDF)](lepidus6007.pdf)** 

## 2. Objetivos de aprendizagem

- Compreender o conceito de *trade-off* entre custo e tempo e sua relação com a tríade escopo–custo–tempo (e qualidade) em projetos.
- Identificar, na literatura e na prática pesquisada pelos autores, quais ferramentas e técnicas as empresas efetivamente utilizam para tratar esse conflito.
- **Transferir** os conceitos do artigo para um projeto real e próprio — o seu TCC — reconhecendo onde as decisões de custo e tempo já estão sendo tomadas, muitas vezes de forma implícita.
- Produzir e justificar decisões de projeto documentadas, com base em critérios e não em intuição.

## 3. Etapa 1 — Leitura dirigida do artigo

Leia o artigo integralmente e responda, com suas próprias palavras (respostas curtas, de 3 a 6 linhas cada). Sempre que usar uma ideia do texto, indique a seção ou o autor citado.

1. Como o artigo define *trade-off* (a partir de Nishi *et al.*, 2006) e por que essa definição implica que **não existe decisão neutra** em um projeto?
2. O artigo, apoiado em Zang, Zou e Qi (2015), divide o dilema tempo × custo em três problemas: **problema de prazo**, **problema de orçamento** e **problema da curva tempo–custo**. Explique cada um e dê um exemplo de projeto de software para cada.
3. Feng e Liu (1997) separam as técnicas de solução em **métodos heurísticos** e **modelos de programação matemática**. Qual a diferença entre eles e qual a limitação apontada para cada um?
4. Nos resultados da pesquisa (Gráfico 3), **74% dos profissionais apontaram o gerenciamento do escopo** como o processo mais importante e **nenhum respondente citou gerenciar tempo e custo**. Qual é a leitura crítica que os autores fazem desse dado? Você concorda? Justifique.
5. Entre os que reconheceram existir o conflito, **69% apontaram maior dificuldade no planejamento do custo** e **78% declararam não utilizar nenhuma técnica** formal de *trade-off*. Em sua opinião, quais são as consequências práticas dessa lacuna para um projeto de software?
6. O **Método do Caminho Crítico (CPM)** foi a técnica mais citada (48%) para determinação de prazos. Explique, em termos simples, por que o caminho crítico é justamente o lugar onde o *trade-off* entre custo e tempo se manifesta.

## 4. Etapa 2 — Relação com o seu projeto de TCC

Esta é a parte principal da atividade. Trate o seu TCC como um **projeto real**, com início, fim, escopo definido, prazo rígido e recursos limitados — exatamente como o artigo caracteriza um projeto (Janovik, 2010; Souto, 2011).

> **Antes de começar, defina o que é "custo" no seu TCC.** Em um projeto acadêmico o custo raramente é apenas dinheiro. Considere, no mínimo: (a) **horas de trabalho** suas e da equipe/orientador — a variável mais escassa; (b) custos financeiros diretos (hospedagem, domínio, APIs pagas, serviços de nuvem, licenças, hardware, deslocamento para coleta de dados); (c) **custo de oportunidade** — o que deixa de ser feito no TCC quando você escolhe fazer outra coisa.

### 4.1 Caracterização do projeto

Apresente em meia página: tema e objetivo do TCC, entregas previstas (produto de software, artigo, apresentação), prazo final e as principais restrições que você já enfrenta.

### 4.2 Cronograma e caminho crítico

Liste de 8 a 12 atividades do seu TCC, com duração estimada (em semanas) e dependências. Identifique o **caminho crítico** — a sequência de atividades cujo atraso atrasa o TCC inteiro. Indique também 2 atividades que possuem folga.

### 4.3 Quadro de trade-offs do seu TCC

Registre **no mínimo quatro** decisões do seu projeto em que ganhar tempo custa algo, ou economizar custo consome tempo. Use o quadro abaixo.

| Decisão / ponto do projeto | Alternativa A (mais rápida) | Alternativa B (mais econômica) | Impacto em tempo e custo | Escolha e justificativa |
|---|---|---|---|---|
| 1. | | | | |
| 2. | | | | |
| 3. | | | | |
| 4. | | | | |

*Quadro 1 — Registro de decisões de trade-off custo × tempo no projeto de TCC.*

**Exemplos de decisões típicas em TCC de ADS** (use como inspiração, não copie): usar um *framework* ou serviço pronto (BaaS, autenticação como serviço, biblioteca de UI) em vez de implementar do zero; contratar hospedagem paga em vez de configurar servidor próprio; reduzir a cobertura de testes automatizados para ganhar semanas; usar dados sintéticos em vez de coletar dados reais em campo; diminuir o número de telas/funcionalidades do MVP; trabalhar sozinho em vez de dividir tarefas que exigiriam integração.

### 4.4 Cenário de compressão de cronograma

Simule o seguinte: **você perdeu 3 semanas** do cronograma (problema de saúde, estágio, retrabalho após banca de qualificação). O prazo final **não** pode ser alterado. Responda no quadro:

| Alternativa de resposta | O que se ganha em tempo | O que se paga (custo, escopo ou qualidade) |
|---|---|---|
| Reduzir escopo do produto | | |
| Aumentar recursos (horas semanais, ajuda de terceiros, ferramentas pagas) | | |
| Executar atividades em paralelo (*fast tracking*) | | |
| Reduzir qualidade/testes/documentação | | |

*Quadro 2 — Análise de alternativas para compressão do cronograma.*

Ao final, **escolha uma alternativa** e justifique com base no artigo, deixando explícito qual conflito você está aceitando.

### 4.5 Confronto com os resultados da pesquisa

Responda de forma honesta e argumentada:

- Assim como os 74% dos profissionais pesquisados, você também vinha priorizando o **escopo** do TCC e tratando prazo e custo como consequência? Que evidências do seu próprio planejamento sustentam sua resposta?
- Você se enquadra nos **78% que não utilizam nenhuma técnica** formal para tratar o *trade-off*? Depois desta atividade, qual técnica ou instrumento (CPM, análise de alternativas, estimativa *bottom-up*, compressão de cronograma, PDCA, registro de lições aprendidas) você passará a adotar no seu TCC, e como?
- Qual dos três problemas de Zang, Zou e Qi (2015) melhor descreve a situação do seu TCC hoje: prazo, orçamento ou curva tempo–custo? Por quê?

## 5. Estrutura e formato do relatório

O relatório deve ser redigido **no formato de artigo científico, seguindo o modelo de publicações da SBC (Sociedade Brasileira de Computação)** — o mesmo template adotado nos TCCs do curso. Além do conteúdo, será avaliada a correta aplicação do modelo, pois esta atividade também serve de treino para a escrita do seu próprio TCC.

### 5.1 Padrão de formatação

- Papel A4, **coluna única**, fonte Times New Roman 12, texto justificado, entrega em **PDF**.
- **Título** centralizado em negrito; abaixo, o nome do autor com afiliação em sobrescrito, a instituição (*Instituto Federal do Paraná (IFPR) – Campus Cascavel*) e o e-mail institucional.
- **Abstract** em inglês (100 a 150 palavras, em itálico e recuado) seguido de **Keywords** (3 a 5 termos); em seguida, **Resumo** em português na mesma extensão, seguido de **Palavras-chave**.
- Seções **numeradas** (1., 2., 2.1., 2.2. …); a seção **Referências**, ao final, não é numerada.
- **Citações no padrão SBC** (autor-data entre colchetes), inseridas no corpo do texto: [Thielmann and Queiroz 2021], [Zang et al. 2015], [Feng and Liu 1997]. Não use notas de rodapé para citar.
- **Tabelas** com legenda **acima** (ex.: "Tabela 1. Decisões de trade-off do projeto") e **figuras** com legenda **abaixo** (ex.: "Figura 1. Cronograma e caminho crítico"). Toda tabela e figura deve ser numerada e **citada no texto** antes de aparecer.
- **Extensão:** 2 a 4 páginas de texto, além de Abstract/Resumo e Referências.
- Recomenda-se produzir o documento no template SBC em LaTeX (Overleaf) ou no modelo *.docx* equivalente disponibilizado pelo professor.

### 5.2 Seções obrigatórias

- **1. Introdução** — tema e objetivo do seu TCC, contexto do problema e por que o *trade-off* entre custo e tempo é relevante nesse projeto. Encerre indicando o objetivo do relatório e como ele está organizado.
- **2. Referencial Teórico** — síntese crítica do artigo (Etapa 1), organizada em subseções, por exemplo: *2.1 Trade-off e a tríade escopo–custo–tempo*; *2.2 Técnicas para o problema tempo–custo*; *2.3 O trade-off na prática das empresas pesquisadas*. Redija em texto corrido, com citações — não como lista de respostas às questões.
- **3. Material e Métodos** — como você analisou o próprio TCC: levantamento das atividades, base das estimativas de duração e de custo, critérios adotados e limitações da análise.
- **4. Resultados e Discussão** — a Etapa 2: cronograma e caminho crítico (Figura 1), o Quadro 1 reproduzido como **Tabela 1**, o Quadro 2 como **Tabela 2**, e a discussão do item 4.5 confrontando seus dados com os resultados da pesquisa do artigo.
- **5. Considerações Finais** — o que muda no planejamento do seu TCC a partir desta leitura, e quais limitações permanecem.
- **Referências** — no padrão SBC (autor, ano, título, veículo), em ordem alfabética, incluindo obrigatoriamente o artigo-base e ao menos uma das obras nele citadas.

## 6. O que será avaliado

- **Compreensão do artigo** — as respostas da Etapa 1 demonstram leitura efetiva, com uso correto dos conceitos e não apenas cópia de trechos.
- **Qualidade da transferência** — os *trade-offs* apresentados são reais, específicos do TCC e verificáveis; não são exemplos genéricos de empresa.
- **Consistência técnica** — cronograma, caminho crítico e estimativas coerentes entre si e com o escopo declarado.
- **Justificativa das decisões** — as escolhas são fundamentadas em critérios explícitos, com o custo da decisão assumido claramente.
- **Redação e aderência ao modelo** — clareza, norma culta e uso correto do template SBC (estrutura de seções, abstract/resumo, citações, numeração e legendas de tabelas e figuras).

---

> **Observação:** não existe resposta certa única nesta atividade. Um relatório que assume "reduzi os testes para entregar no prazo, e o custo disso é maior risco de defeitos na apresentação da banca" vale mais do que um relatório que afirma ter conseguido otimizar tempo, custo e qualidade ao mesmo tempo — que é exatamente a ilusão que o artigo desmonta.
