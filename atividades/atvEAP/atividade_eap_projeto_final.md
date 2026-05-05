# Atividade Construção da EAP do Projeto Final

## 1. Contexto da atividade

Na atividade anterior, cada estudante elaborou a primeira versão do **Termo de Abertura do Projeto (TAP)** do seu projeto final.

Nesta nova etapa, o estudante deverá dar continuidade ao planejamento do projeto, utilizando o TAP como ponto de partida para construir a **Estrutura Analítica do Projeto (EAP)**.

A EAP deverá organizar, de forma hierárquica, os principais **entregáveis** necessários para que o projeto seja concluído com sucesso.

> **Importante:** nesta atividade, o estudante **não deverá refazer o TAP**.  
> O TAP já produzido deverá ser utilizado apenas como base para identificar o escopo, os objetivos, as entregas principais, as restrições e as condições de sucesso do projeto.

---

## 2. Materiais de apoio

1. TAP já elaborado na atividade anterior;
2. Arquivo da aula: **Aula 04 — Estruturando o Projeto: Estrutura Analítica do Projeto (EAP)**;
3. Documento-base do projeto anual: **Projeto Final (TADS – Último Ano) — Mobile + API (2026)**;
4. Anotações e discussões realizadas em sala.

---

## 3. Objetivo da atividade

Construir a **Estrutura Analítica do Projeto (EAP)** do projeto final individual, organizando o trabalho em partes menores e mais claras.

Ao final da atividade, o estudante deverá demonstrar que compreende:

- a relação entre TAP, escopo e EAP;
- a diferença entre entregáveis e atividades;
- a organização hierárquica de uma EAP;
- a importância da EAP para o planejamento do cronograma, dos recursos e das responsabilidades;
- os principais entregáveis técnicos exigidos para o projeto final.

---

## 4. O que é esperado nesta atividade

Cada estudante deverá criar uma EAP para o seu próprio projeto final, considerando o tema escolhido no TAP.

A EAP deve responder à seguinte pergunta:

> **O que precisa ser entregue para que o meu projeto seja considerado concluído?**

A estrutura deve apresentar o projeto de forma hierárquica, partindo do nome geral do projeto até chegar aos entregáveis menores.

---

## 5. Requisitos obrigatórios da EAP

A EAP deve conter, obrigatoriamente:

### 5.1 Identificação do projeto

- nome do estudante;
- nome do projeto;
- breve descrição do projeto;
- referência ao TAP já elaborado.

### 5.2 Estrutura hierárquica

A EAP deve possuir, no mínimo, **três níveis**:

```text
1. Nome do Projeto
   1.1 Entrega principal
       1.1.1 Entregável específico
       1.1.2 Entregável específico
```

O estudante poderá utilizar um quarto nível, caso seja necessário detalhar melhor alguma parte do projeto.

### 5.3 Foco em entregáveis

Os itens da EAP devem representar **entregáveis**, e não apenas ações genéricas.

Exemplo inadequado:

```text
1.3 Fazer o sistema
```

Exemplo mais adequado:

```text
1.3 Desenvolvimento do aplicativo mobile
    1.3.1 Tela de login
    1.3.2 Tela de cadastro de usuário
    1.3.3 Tela de listagem de registros
```

### 5.4 Coerência com o TAP

A EAP deve estar alinhada ao TAP entregue anteriormente.

Isso significa que os seguintes elementos do TAP devem aparecer de forma coerente na EAP:

- objetivo do projeto;
- escopo;
- entregas principais;
- restrições;
- recursos necessários;
- requisitos técnicos obrigatórios;
- condições de sucesso.

---

## 6. Entregáveis técnicos mínimos que devem aparecer na EAP

Como o projeto final possui um padrão técnico obrigatório, a EAP deverá contemplar entregáveis relacionados a:

- planejamento e levantamento de requisitos;
- prototipação das telas;
- aplicação mobile em **React Native + Expo**;
- API em **NestJS**;
- banco de dados **Postgres**;
- uso de **Prisma**;
- persistência local com **SQLite**;
- autenticação com **JWT**;
- controle de acesso com **RBAC**;
- sincronização **push/pull**;
- funcionalidade de **upload de arquivo**;
- no mínimo **4 entidades principais**;
- testes;
- integração contínua (**CI**);
- documentação técnica;
- apresentação final do projeto.

> **Atenção:** esses itens não precisam aparecer exatamente com esses nomes, mas devem estar representados de forma clara na EAP.

---

## 7. Sugestão de organização da EAP

A organização abaixo é apenas uma sugestão.  
Cada estudante deve adaptar a estrutura de acordo com o seu projeto.

```text
1. Nome do Projeto
   1.1 Planejamento do projeto
       1.1.1 Revisão do TAP
       1.1.2 Definição do escopo
       1.1.3 Levantamento dos requisitos
       1.1.4 Definição das entidades principais

   1.2 Prototipação
       1.2.1 Protótipo da tela de login
       1.2.2 Protótipo das telas principais
       1.2.3 Validação inicial do fluxo de uso

   1.3 Desenvolvimento da API
       1.3.1 Estrutura inicial do projeto NestJS
       1.3.2 Configuração do Postgres
       1.3.3 Configuração do Prisma
       1.3.4 CRUD das entidades principais
       1.3.5 Autenticação com JWT
       1.3.6 Controle de acesso com RBAC
       1.3.7 Upload de arquivo

   1.4 Desenvolvimento do aplicativo mobile
       1.4.1 Estrutura inicial do projeto React Native + Expo
       1.4.2 Navegação entre telas
       1.4.3 Telas de cadastro e consulta
       1.4.4 Integração com a API
       1.4.5 Persistência local com SQLite
       1.4.6 Sincronização push/pull

   1.5 Testes e qualidade
       1.5.1 Testes da API
       1.5.2 Testes do aplicativo mobile
       1.5.3 Correção de falhas
       1.5.4 Configuração da integração contínua

   1.6 Documentação e entrega
       1.6.1 Documentação técnica
       1.6.2 Manual básico de uso
       1.6.3 Organização do repositório
       1.6.4 Apresentação final
```

> **Observação:** a estrutura acima não deve ser simplesmente copiada.  
> Ela serve apenas como referência para orientar a construção da EAP de cada projeto.

---

## 8. Representação visual da EAP

Além da estrutura textual hierárquica, o estudante deverá apresentar uma versão visual da EAP.

A representação visual deverá ser feita da seguinte forma:

- ferramenta online de diagramas (em construção);

---

## 9. Cuidados importantes

Ao elaborar a EAP, observe os seguintes cuidados:

1. A EAP deve ser baseada no escopo do projeto definido no TAP.
2. Cada item deve representar uma entrega clara.
3. A estrutura não deve ser uma lista solta de tarefas.
4. Os entregáveis devem estar organizados de forma hierárquica.
5. Cada item subordinado deve pertencer a apenas um item superior.
6. Os principais requisitos técnicos do projeto final não podem ficar de fora.
7. A EAP não é o cronograma do projeto.
8. Não é necessário colocar datas em cada item da EAP.
9. Não copie a estrutura de colegas.
10. Não utilize modelos prontos da internet sem adaptação ao seu projeto.

---

## 10. Questões de reflexão

Junto com a EAP, responda brevemente às questões abaixo:

1. Como o TAP ajudou na construção da EAP?
2. Quais foram as principais entregas identificadas para o seu projeto?
3. Qual parte do projeto exigiu maior detalhamento na EAP? Justifique.
4. Quais entregáveis técnicos obrigatórios aparecem na sua EAP?
5. Qual é a diferença entre a sua EAP e um cronograma?
6. O que poderia acontecer se algum entregável importante ficasse fora da EAP?

> **Importante:** respostas muito curtas, sem explicação, não serão consideradas completas.

---

## 11. Entrega da atividade

A entrega deverá ser realizada no **Google Classroom** da disciplina de **Gerenciamento de Projetos**.

O estudante deverá entregar **um único arquivo PDF** contendo:

1. identificação do estudante e do projeto;
2. breve descrição do projeto;
3. EAP textual em formato hierárquico;
4. EAP visual;
5. respostas das questões de reflexão.

A data de entrega será aquela definida pelo professor no Google Classroom.

> **Atenção:** trabalhos entregues com atraso terão **desconto de 1,0 ponto por dia de atraso**.

---

## 12. Critérios de avaliação

| Critério | Valor |
|---|---:|
| Coerência entre TAP, escopo e EAP | 2,0 |
| Organização hierárquica da EAP | 2,0 |
| Clareza e qualidade dos entregáveis | 2,0 |
| Inclusão dos requisitos técnicos obrigatórios | 2,0 |
| Representação visual da EAP | 1,0 |
| Respostas às questões de reflexão | 1,0 |
| **Total** | **10,0** |

---

## 13. Conceitos

| Conceito | Faixa de nota correspondente |
|---|---|
| A | 9,0 – 10,0 |
| B | 7,0 – 8,9 |
| C | 5,0 – 6,9 |
| D | Abaixo de 4,9 |

---

## 14. Observações sobre autoria

Cada estudante deverá produzir sua própria EAP, com base no seu próprio projeto.

EAPs com estrutura idêntica, texto copiado de colegas, cópia de modelos prontos ou indícios de plágio poderão receber **conceito D**.

Também será realizada análise de indícios de uso indevido de agentes de IA. Caso seja identificado uso que substitua a autoria do estudante, a atividade poderá receber **conceito D**.

---

## 15. Síntese da atividade

Nesta atividade, o estudante deverá transformar o planejamento inicial apresentado no TAP em uma estrutura organizada de entregáveis.

A EAP será a base para as próximas etapas do gerenciamento do projeto, especialmente para a construção do cronograma, a definição de responsabilidades, a estimativa de esforço e o acompanhamento das entregas.
