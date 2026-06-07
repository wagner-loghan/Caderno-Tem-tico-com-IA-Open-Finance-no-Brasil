# Caderno Temático com IA — Open Finance no Brasil

> Projeto desenvolvido como parte do Bootcamp Bradesco + DIO  
> Ferramenta principal: [NotebookLM](https://notebooklm.google.com/) (Google)


## 1. Por que escolhi esse tema?

Quando comecei a pensar em qual assunto financeiro estudar, quis fugir do óbvio. Juros compostos e orçamento pessoal são temas importantes, mas qualquer livro de finanças cobre isso. O que me chamou atenção foi uma pergunta diferente: **como os bancos estão mudando por dentro por causa da tecnologia?**

O Open Finance é a resposta mais concreta que encontrei. É uma mudança real, em andamento agora no Brasil, que afeta diretamente como as pessoas se relacionam com os bancos e como os bancos competem entre si. Para quem está num bootcamp voltado à tecnologia e ao setor financeiro, entender esse movimento é praticamente obrigatório.


## 2. Objetivos de Estudo

Antes de montar o caderno no NotebookLM, determinei três perguntas que queria conseguir responder com clareza ao final:

- O que é Open Finance e como ele funciona na prática no Brasil?
- Quem regula, quem participa e quem se beneficia?
- Como a inteligência artificial se encaixa nesse ecossistema?

Esses objetivos guiaram tanto a escolha das fontes quanto as perguntas que fiz à IA durante os testes.


## 3. Fontes Utilizadas

Selecionei cinco fontes abertas, todas gratuitas e com credibilidade institucional. Todas foram carregadas no NotebookLM para a construção do caderno.

| # | Fonte | Descrição | Link |
|---|-------|-----------|------|
| 1 | Banco Central do Brasil | Portal oficial do Open Finance Brasil com apresentação do sistema, fases de implementação e participantes | [acessar](https://www.bcb.gov.br/estabilidadefinanceira/openfinance) |
| 2 | Banco Central do Brasil | FAQ do Open Finance para o consumidor — explica em linguagem simples o que muda para quem usa banco | [acessar](https://www.bcb.gov.br/meubc/faqs/s/open-finance) |
| 3 | Banco Central do Brasil | Relatório de Economia Bancária 2023 — contém capítulo dedicado ao Open Finance e seus efeitos no mercado (PDF aberto) | [acessar](https://www.bcb.gov.br/content/publicacoes/relatorioeconomiabancaria/reb2023p.pdf) |
| 4 | FEBRABAN | Pesquisa FEBRABAN de Tecnologia Bancária 2023 — dados sobre digitalização dos bancos brasileiros e adoção de open banking | [acessar](https://portal.febraban.org.br/pagina/3106/1117/pt-br/pesquisa) |
| 5 | Gov.br — Ministério da Fazenda | Documento explicativo sobre o Sistema Financeiro Aberto e o papel do Banco Central como regulador | [acessar](https://www.bcb.gov.br/estabilidadefinanceira/exibenormativo?tipo=Resolu%C3%A7%C3%A3o%20BCB&numero=400) |

> **Critério de seleção:** priorizei fontes institucionais e regulatórias porque o Open Finance é um tema em que a precisão importa. Opinião de blog ou artigo genérico poderia distorcer o entendimento.


## 4. Engenharia de Prompts — O Processo por Trás dos Resultados

Esta seção é a parte mais Direta do projeto. Documentei não só as perguntas que funcionaram, mas também o que não funcionou e como ajustei os prompts.


### 4.1 Prompts Iniciais — Tentativas e Erros

**Tentativa 1 — Prompt muito genérico**

```
O que é Open Finance?
```

**Resposta obtida:** A IA deu uma definição curta e superficial, sem estar ancorada nas fontes carregadas. Parecia uma resposta de enciclopédia, não um resumo do material que eu tinha estudado.

**Problema identificado:** O prompt não direcionava a IA para usar as fontes do caderno. Ela recorreu ao conhecimento geral, ignorando os documentos.

**Ajuste feito:** Passei a referenciar os documentos diretamente nas perguntas.


**Tentativa 2 — Prompt mais direcionado**

```
Com base nas fontes carregadas, explique o que é Open Finance no Brasil 
e quais foram as fases de implementação definidas pelo Banco Central.
```

**Resposta obtida:** Muito melhor. A IA trouxe as quatro fases do Open Finance com referência direta ao portal do Banco Central. A resposta estava ancorada no material real. **OBS**: *Problema parcial identificado*: Mesmo com as fontes a IA não achou informação suficiente, apenas uma referencia com potencial de afirmidade de 80%, acionei a pergunta padrão sugerida pelo notebook que procurou na web, o restante da informação requerida pela pergunta do prompt. PS: Adicionei mais 8 fontes para obter poder de informação complementar.  

**O que aprendi:** Pedir que a IA use as fontes carregadas faz uma diferença enorme na qualidade e na confiabilidade da resposta, mas deve-se atenta-se para as fontes e seu potencial de confiabilidade.


### 4.2 Prompts Estratégicos: Os Que Funcionaram Bem

**Prompt de conceito:**
```
Explique o conceito de portabilidade de dados no Open Finance como 
se estivesse explicando para alguém que nunca usou aplicativo de banco.
```
*Por que funciona:* Forçar uma linguagem simples revela se a IA realmente entendeu o conceito ou se está só repetindo termos técnicos.


**Prompt de comparação:**
```
Qual é a diferença entre Open Banking e Open Finance? 
O que mudou de uma fase para a outra no contexto brasileiro?
```
*Por que funciona:* Perguntas comparativas forçam a IA a distinguir conceitos próximos, o que ajuda a fixar o aprendizado.


**Prompt de impacto prático:**
```
De que forma o Open Finance beneficia o consumidor comum no dia a dia? 
Dê exemplos concretos baseados nas fontes disponíveis.
```
*Por que funciona:* Pedir exemplos concretos evita respostas vagas e conecta o conceito com a realidade.


**Prompt crítico:**
```
Quais são os principais riscos do Open Finance para o consumidor, 
especialmente em relação à privacidade e segurança de dados?
```
*Por que funciona:* Todo tema tem dois lados. Perguntar sobre riscos demonstra pensamento crítico e traz um ângulo que manuais oficiais tendem a suavizar.


**Prompt de conexão com IA:**
```
Como a inteligência artificial está sendo usada dentro do ecossistema 
de Open Finance pelos bancos brasileiros?
```
*Por que funciona:* Conecta o tema financeiro com o tema central do bootcamp, mostrando que os assuntos se completam.


### 4.3 Dificuldades Encontradas (Troubleshooting)

| Problema | Causa | Solução |
|----------|-------|---------|
| Respostas genéricas sem usar as fontes | Prompt sem instrução clara para referenciar o material | Adicionar "com base nas fontes carregadas" ou "segundo os documentos disponíveis" |
| Resposta muito longa e difícil de usar | Pergunta aberta demais | Especificar formato: "explique em até 5 pontos" ou "faça um resumo de 3 parágrafos" |
| IA misturou informações de fases diferentes | Pergunta não delimitou o escopo temporal | Incluir a fase ou o período no próprio prompt |
| Glossário com definições muito técnicas | A IA manteve o tom dos documentos institucionais | Pedir explicitamente: "use linguagem simples, sem jargão" |


## 5. Miniguia de Estudo: Entrega Final


### 5.1 Resumos Estruturados

**O que é Open Finance**

Open Finance é um sistema criado e regulamentado pelo Banco Central do Brasil que permite que pessoas e empresas autorizem o compartilhamento dos seus dados financeiros entre diferentes instituições. Em linguagem simples: se você tem conta em dois bancos e quer que um deles veja seu histórico no outro para te oferecer uma condição melhor de crédito, o Open Finance torna isso possível — com a sua autorização.


**Como surgiu e como está organizado**

O sistema foi implementado em fases a partir de 2021. Começou pelo compartilhamento de informações sobre produtos e serviços dos bancos, avançou para o compartilhamento de dados de clientes e chegou ao estágio atual, que inclui pagamentos, investimentos, câmbio e seguros. O nome evoluiu de Open Banking para Open Finance justamente porque o escopo foi ampliado além das contas e empréstimos.


**Quem regula e quem participa**

O Banco Central é o regulador principal. A participação é obrigatória para bancos, financeiras e demais instituições autorizadas a funcionar pelo BCB. Fintechs e empresas de tecnologia financeira também participam, o que aumenta a competição e, na teoria, beneficia o consumidor com mais opções e preços melhores.


**O papel da inteligência artificial nesse ecossistema**

Com o Open Finance, os bancos passaram a ter acesso a um volume muito maior de dados sobre o comportamento financeiro dos clientes. A IA entra para processar esses dados e gerar análises de crédito mais precisas, ofertas personalizadas de produtos e detecção de fraudes em tempo real. O Open Finance sem IA seria apenas uma troca de planilhas. Com IA, vira inteligência de negócio.


**Benefícios e riscos**

Do lado positivo: mais concorrência entre bancos, melhores condições de crédito para quem tem bom histórico, portabilidade real de conta e facilidade para comparar produtos. Do lado dos riscos: preocupações com privacidade, possibilidade de uso indevido dos dados por terceiros e o desafio de garantir segurança num sistema com muitos participantes conectados.


### 5.2 Glossário

| Termo | O que significa na prática |
|-------|---------------------------|
| **Open Finance** | Sistema que permite o compartilhamento de dados financeiros entre instituições, com autorização do cliente |
| **Open Banking** | Fase inicial do Open Finance, focada em dados de contas e crédito — hoje expandida |
| **API** | "Porta" tecnológica que permite que sistemas diferentes se comuniquem e troquem dados com segurança |
| **Consentimento** | Autorização formal que o cliente dá para que seus dados sejam compartilhados. Pode ser revogada a qualquer momento |
| **Portabilidade de dados** | Direito do cliente de levar seu histórico financeiro para outra instituição |
| **Fintechs** | Empresas de tecnologia que oferecem serviços financeiros, geralmente com menos burocracia que bancos tradicionais |
| **LGPD** | Lei Geral de Proteção de Dados — lei brasileira que regula como dados pessoais podem ser coletados e usados |
| **Banco Central (BCB)** | Autoridade monetária do Brasil, responsável por regular e supervisionar o sistema financeiro |
| **Ecossistema financeiro** | Conjunto de todas as instituições, regras e tecnologias que fazem o sistema financeiro funcionar junto |
| **Crédito personalizado** | Oferta de empréstimo ou financiamento baseada no histórico real do cliente, não em médias genéricas |


### 5.3 Prompts Reutilizáveis para Revisão Futura

Estes prompts podem ser usados em qualquer sessão futura no NotebookLM ou em outra ferramenta de IA para revisar o tema com qualidade.


**Para revisar conceitos:**
```
Com base nas fontes carregadas, explique [conceito] de forma simples, 
como se fosse para alguém que nunca trabalhou com finanças.
```

**Para criar resumos de estudo:**
```
Faça um resumo em tópicos sobre [tema específico] usando apenas 
as informações presentes nas fontes deste caderno.
```

**Para aprofundar um ponto:**
```
Quais são as implicações práticas de [tema] para o consumidor brasileiro 
de acordo com os documentos disponíveis?
```

**Para pensar criticamente:**
```
Quais são os argumentos a favor e contra [tema] presentes nas fontes? 
Apresente os dois lados de forma equilibrada.
```

**Para conectar com tecnologia:**
```
De que forma a inteligência artificial e os dados abertos se relacionam 
com [tema] no contexto do mercado financeiro brasileiro?
```

**Para montar glossário:**
```
Liste os 10 termos técnicos mais importantes sobre [tema] presentes 
nas fontes e explique cada um em uma frase simples.
```

**Para simular uma prova ou entrevista:**
```
Elabore 5 perguntas sobre [tema] com nível de dificuldade intermediário, 
como se fosse uma avaliação para uma vaga na área financeira.
```


## 6. Reflexão Final

Trabalhar com o NotebookLM neste projeto mudou um pouco minha forma de estudar. A diferença não está na ferramenta em si, mas na necessidade de organizar o pensamento antes de fazer a pergunta. Um prompt ruim gera uma resposta ruim, independente de quão boa seja a IA. Isso me fez perceber que a habilidade mais importante aqui não é técnica — é saber o que você quer aprender e conseguir traduzir isso em uma pergunta bem feita.

O tema de Open Finance também me surpreendeu. Parece distante no começo, mas quando você entende que está falando de dados, APIs, regulação e inteligência artificial num mercado de 200 milhões de pessoas, fica claro que é um dos assuntos mais relevantes para quem quer atuar na intersecção entre tecnologia e finanças.


## 7. Ferramentas e Tecnologias Utilizadas

- [NotebookLM](https://notebooklm.google.com/):Google (organização do caderno e testes de prompts)
- [GitHub](https://github.com/): versionamento e publicação do projeto
- Fontes institucionais abertas: Banco Central do Brasil, FEBRABAN, Gov.br


***Projeto desenvolvido para o Bootcamp Bradesco + DIO Trilha de Inteligência Artificial***
