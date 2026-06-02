# Estudo de Caso: Abertura da Cafeteria "Grão & Aroma"

### Estrutura Analítica do Projeto (EAP) e Diagrama de Redes

---

## 1. Objetivos de aprendizagem

Ao concluir esta atividade, você deverá ser capaz de:

- Decompor o escopo de um projeto em uma Estrutura Analítica do Projeto (EAP) organizada em níveis.
- Diferenciar entregáveis (pacotes de trabalho) de atividades de execução.
- Sequenciar atividades a partir de suas relações de dependência e construir um diagrama de redes.
<!-- - Calcular datas de início e término, folgas e a duração total do projeto.
- Identificar e interpretar o caminho crítico. -->

## 2. Instruções gerais

1. Leia o caso com atenção antes de começar.
2. A atividade deve ser feita individualmente.
<!--3. Você pode usar papel, quadro, software de sua preferência (ex.: planilha, ferramentas de diagrama) ou desenhar à mão.
4. Entregue os dois produtos solicitados: a EAP (Parte 1) e o diagrama de redes com os cálculos (Parte 2).
5. Justifique suas escolhas sempre que solicitado. Não existe uma única EAP "correta" — existe coerência com o escopo. -->

## 3. O caso

Mariana decidiu realizar um sonho antigo: abrir uma cafeteria de bairro chamada **"Grão & Aroma"**, em um ponto comercial que ela acabou de alugar. O espaço precisa de uma reforma completa antes da abertura, e ela quer inaugurar com um pequeno evento para a vizinhança.

Para organizar o trabalho, Mariana mapeou tudo o que precisa ser feito. Primeiro, ela vai elaborar um plano de negócios com o orçamento geral, que servirá de base para todas as demais decisões. Só depois disso ela conseguirá dar entrada nas licenças e alvarás na prefeitura e na vigilância sanitária, contratar a empresa que fará a reforma e também começar a definir o cardápio e negociar com fornecedores.

A reforma do espaço (parte elétrica, hidráulica e pintura) só pode começar quando as licenças estiverem aprovadas e a empresa de reforma estiver contratada. Com o espaço reformado, será possível comprar e instalar os equipamentos (máquinas de café, geladeiras) e, em paralelo, comprar e montar o mobiliário (balcão, mesas e cadeiras).

A contratação da equipe pode ser iniciada assim que as licenças saírem, mas o treinamento dos funcionários depende de a equipe já estar contratada e de os equipamentos já estarem instalados — afinal, eles precisam treinar nas máquinas reais.

A campanha de marketing e divulgação depende do cardápio definido e do mobiliário montado (para que se possa fotografar o ambiente). Por fim, o evento de inauguração só acontece quando a equipe estiver treinada e a campanha de marketing tiver sido realizada.

## 4. Parte 1 — Estrutura Analítica do Projeto (EAP)

Com base no caso, construa a EAP do projeto "Abertura da Cafeteria Grão & Aroma". Siga as orientações:

1. Coloque o projeto no nível mais alto (nível 0 / 1).
2. Agrupe o trabalho em fases ou entregáveis principais (nível 2). 
3. Decomponha cada item em pacotes de trabalho (nível 3) — os entregáveis menores e gerenciáveis.
4. Use a regra dos 100%: a soma dos níveis inferiores deve representar todo o trabalho do nível acima, nem mais, nem menos.
5. Numere os itens de forma hierárquica (1, 1.1, 1.1.1, …).

> **Dica:** os itens da EAP devem ser entregáveis (substantivos), e não ações. Escreva "Equipe treinada" ou "Treinamento da equipe", e não "Treinar a equipe todos os dias".

## 5. Parte 2 — Diagrama de Redes

A tabela abaixo lista as atividades de execução do projeto, com suas durações estimadas e suas predecessoras (as atividades que precisam terminar antes que ela comece).

| ID | Atividade | Duração (dias) | Predecessoras |
|:--:|---|:--:|:--:|
| A | Elaborar plano de negócios e orçamento | 5 | — |
| B | Obter licenças e alvarás junto à prefeitura/vigilância | 10 | A |
| C | Contratar empresa de reforma | 4 | A |
| D | Executar a reforma (elétrica, hidráulica, pintura) | 15 | B, C |
| E | Comprar e instalar equipamentos (máquinas, geladeiras) | 8 | D |
| F | Comprar e montar mobiliário (balcão, mesas, cadeiras) | 6 | D |
| G | Selecionar e contratar a equipe | 7 | B |
| H | Treinar a equipe | 5 | E, G |
| I | Definir cardápio e fechar fornecedores | 6 | A |
| J | Planejar e executar a campanha de marketing | 9 | F, I |
| K | Realizar o evento de inauguração | 2 | H, J |

Com base nessa tabela, faça o que se pede:

1. Desenhe o diagrama de redes, ligando as atividades conforme as predecessoras.
<!-- 2. Faça o cálculo para frente (*forward pass*) e determine o **Início Cedo** e o **Término Cedo** de cada atividade.
3. Faça o cálculo para trás (*backward pass*) e determine o **Início Tarde** e o **Término Tarde** de cada atividade.
4. Calcule a **folga total** de cada atividade (Folga = Início Tarde − Início Cedo).
5. Identifique o **caminho crítico** e informe a **duração total** do projeto.
6. Responda: o que aconteceria com o prazo final se a atividade **D** (reforma) atrasasse 3 dias? E se a atividade **G** (contratação da equipe) atrasasse 3 dias? Justifique usando o conceito de folga.

> **Convenção de cálculo sugerida:** considere que o projeto começa no instante 0. Assim, o Início Cedo da primeira atividade é 0 e o Término Cedo é igual à duração. Mantenha a mesma convenção em toda a rede. -->

## 6. O que entregar

- Diagrama da EAP com a numeração hierárquica (Parte 1).
- Diagrama de redes desenhado.
<!-- - Indicação do caminho crítico e da duração total do projeto.
- Respostas às perguntas de interpretação (item 6 da Parte 2). -->

---