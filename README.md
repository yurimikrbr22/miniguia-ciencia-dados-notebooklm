# Miniguia de Ciência de Dados com NotebookLM

Projeto do desafio da DIO sobre o uso de IA como ferramenta de aprendizagem ativa. Criei um caderno no NotebookLM sobre **Introdução à Ciência de Dados**, testei prompts, registrei os problemas que apareceram e montei um miniguia de estudo com resumos, glossário e prompts reutilizáveis.

**Caderno temático:** *Ciência de Dados do Zero: Primeiros Princípios com Python*

---

## Contexto e objetivos

Escolhi **Introdução à Ciência de Dados** como tema e usei o NotebookLM para estudar, organizar e revisar o conteúdo a partir de fontes que eu mesmo selecionei.

O que eu queria com este material:

* entender os conceitos básicos e as etapas do processo, do dado bruto até a avaliação do modelo;
* diferenciar métodos descritivos de métodos preditivos;
* entender por que avaliar modelos e pensar na ética dos dados são partes do processo;
* testar prompts diferentes e registrar o que funcionou e o que não funcionou;
* deixar prompts prontos para revisões futuras.

---

## Curadoria de fontes

Cinco das fontes abertas que usei no caderno:

| Fonte                                                                                | Para que usei        |
| ------------------------------------------------------------------------------------ | -------------------- |
| [Statistical data type](https://en.wikipedia.org/wiki/Statistical_data_type)         | tipos de dados       |
| [Data cleansing](https://en.wikipedia.org/wiki/Data_cleansing)                       | limpeza e preparação |
| [Exploratory data analysis](https://en.wikipedia.org/wiki/Exploratory_data_analysis) | análise exploratória |
| [K-means clustering](https://en.wikipedia.org/wiki/K-means_clustering)               | agrupamento          |
| [Linear regression](https://en.wikipedia.org/wiki/Linear_regression)                 | regressão e previsão |

O caderno também tem fontes complementares em **PDFs, vídeos e arquivos do Google Drive**. Listei somente estas cinco aqui para documentar uma amostra da curadoria realizada.

---

## Prompts testados

Nos dois prompts abaixo usei duas instruções fixas: trabalhar **somente com as fontes selecionadas** e escrever **"[não encontrado nas fontes]"** quando o assunto não estivesse nelas.

Essa estratégia foi utilizada para verificar quais informações estavam apoiadas pelas fontes e identificar conteúdos que não estavam disponíveis no material selecionado.

### Prompt 1: mapa mental

```text
Com base exclusivamente nas fontes selecionadas neste caderno, crie um mapa mental hierárquico (texto com marcadores indentados, até 4 níveis) sobre Introdução à Ciência de Dados.

Nó central: Ciência de Dados

Ramos principais:
1. Fundamentos: ciência de dados x análise de dados, Big Data, habilidades do cientista de dados, ferramentas
2. Ciclo de vida e etapas do processo, do dado bruto à decisão
3. Tipos de dados e preparação: limpeza, dados faltantes (imputação), outliers
4. Análise exploratória: estatística descritiva e visualização
5. Modelos descritivos: PCA, K-means, agrupamento hierárquico
6. Modelos preditivos: regressão linear, regressão logística, Naive Bayes, árvores de decisão
7. Avaliação de modelos: matriz de confusão, RMSE, treino e teste, viés e variância
8. Limitações, ética e pensamento crítico
9. Aplicações em empresas e negócios

Regras:
- Nós com no máximo 6 palavras.
- Em cada técnica, diga para que serve, quando usar e uma limitação.
- Se um ramo não estiver nas fontes selecionadas, escreva "[não encontrado nas fontes]".
- No final, liste as 3 conexões mais importantes entre ramos diferentes.
```

### Prompt 2: apresentação

```text
Com base exclusivamente nas fontes selecionadas neste caderno, crie uma apresentação de 10 a 12 slides sobre Introdução à Ciência de Dados, para iniciantes sem conhecimento de programação.

Sequência sugerida: capa; objetivos; ciência de dados x análise de dados; ciclo de vida e etapas do processo; tipos de dados e preparação; análise exploratória; modelos descritivos; modelos preditivos; avaliação de modelos; ética e pensamento crítico; resumo com 5 pontos principais.

Regras:
- Título claro e no máximo 4 tópicos curtos por slide.
- Um exemplo prático ou analogia simples quando fizer sentido.
- Notas do apresentador com 2 ou 3 frases.
- Não invente conteúdo. Se algo não estiver nas fontes selecionadas, sinalize.
```

---

## Cicatrizes e troubleshooting

Cheguei à versão final na **terceira tentativa**.

### 1ª tentativa: teste inicial

Algumas fontes estavam repetidas e outras davam erro **404**. Conferi os links um por um, tirei os repetidos e troquei os que não abriam.

### 2ª tentativa: PDFs

Tentei ampliar o material com arquivos PDF, mas alguns deram erro no NotebookLM. Revisei os arquivos e procurei alternativas que funcionassem.

### 3ª tentativa: versão oficial

Revisei novamente as fontes e consolidei o material que utilizo neste projeto.

### O que aprendi

Usar IA para estudar não é só fazer boas perguntas. A qualidade das respostas depende também da qualidade das fontes, então vale conferir cada uma antes de perguntar:

**selecionar → verificar → testar → corrigir → consolidar.**

Esse processo mostrou a importância da curadoria de fontes e do troubleshooting durante o uso de ferramentas de IA.

---

# Miniguia de estudo

## Resumos

### O que é Ciência de Dados

Área que combina estatística, matemática e computação para analisar dados, gerar conhecimento e apoiar decisões.

### Preparação dos dados

Antes de analisar ou modelar, é preciso limpar os dados, tratar valores ausentes, encontrar inconsistências e identificar outliers. Dados inadequados podem comprometer as etapas seguintes.

### Análise exploratória

Serve para entender os dados antes de modelar, usando estatística descritiva, tabelas e gráficos para identificar padrões e valores atípicos.

### Métodos descritivos

Buscam estruturas e padrões nos dados sem necessariamente prever um resultado específico.

Exemplos:

* PCA;
* K-means;
* agrupamento hierárquico.

### Métodos preditivos

Usam os dados disponíveis para estimar ou classificar resultados.

Exemplos:

* regressão linear;
* regressão logística;
* Naive Bayes;
* árvores de decisão;
* florestas aleatórias.

### Aprendizado de máquina

Algoritmos que identificam padrões nos dados.

No aprendizado **supervisionado**, os exemplos possuem uma resposta esperada.

No aprendizado **não supervisionado**, o modelo procura padrões sem uma resposta previamente definida.

### Avaliação de modelos

Depois de construir um modelo, é preciso medir seu desempenho. Para isso, podem ser utilizados dados de treino e teste e métricas como matriz de confusão e RMSE.

Também fazem parte desse processo conceitos como **viés e variância**.

### Limitações e pensamento crítico

Uma resposta que parece correta pode vir de fontes inadequadas ou de dados insuficientes. Isso vale para modelos e também para ferramentas de IA, portanto é necessário validar as informações.

### Ética

Trabalhar com dados envolve questões relacionadas à privacidade, segurança e aos impactos das decisões tomadas a partir deles.

---

## Glossário

| Termo                              | Definição resumida                                                                                           |
| ---------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| **Big Data**                       | Grandes volumes de dados, com características complexas, que podem exigir métodos e tecnologias específicas. |
| **Ciência de Dados**               | Uso de métodos matemáticos, estatísticos e computacionais para gerar conhecimento a partir de dados.         |
| **Análise de Dados**               | Exame dos dados para identificar informações, padrões e relações.                                            |
| **EDA**                            | Análise exploratória de dados, utilizada para compreender características e padrões de um conjunto de dados. |
| **Outlier**                        | Observação muito diferente das demais.                                                                       |
| **Imputação**                      | Preenchimento ou tratamento de valores ausentes.                                                             |
| **Clustering**                     | Agrupamento de objetos de acordo com suas características ou semelhanças.                                    |
| **K-means**                        | Algoritmo de agrupamento que organiza dados em grupos.                                                       |
| **PCA**                            | Técnica de redução de dimensionalidade que busca preservar informações relevantes dos dados.                 |
| **Regressão linear**               | Método que modela relações entre variáveis e pode ser utilizado para previsões numéricas.                    |
| **Regressão logística**            | Método utilizado principalmente em problemas de classificação.                                               |
| **Naive Bayes**                    | Classificador probabilístico baseado no teorema de Bayes.                                                    |
| **Aprendizado supervisionado**     | Aprende a partir de exemplos que possuem uma resposta esperada.                                              |
| **Aprendizado não supervisionado** | Busca padrões nos dados sem respostas previamente definidas.                                                 |
| **Matriz de confusão**             | Tabela utilizada para analisar acertos e erros de uma classificação.                                         |
| **RMSE**                           | Métrica utilizada para medir erros em previsões numéricas.                                                   |
| **Viés**                           | Erro associado a simplificações ou limitações sistemáticas de um modelo.                                     |
| **Variância**                      | Sensibilidade do modelo às variações nos dados utilizados para treinamento.                                  |

---

## Prompts reutilizáveis

Troque `[CONCEITO]` e `[TEMA]` pelo assunto que quiser revisar.

### Revisão de um conceito

```text
Com base exclusivamente nas fontes fornecidas, explique [CONCEITO] para um iniciante.

Organize em:
1. definição;
2. como funciona;
3. exemplo simples;
4. aplicação;
5. limitação;
6. relação com outros conceitos estudados.

Se a informação não estiver nas fontes, responda:
"Não encontrado nas fontes".
```

### Comparação

```text
Com base exclusivamente nas fontes fornecidas, compare [CONCEITO A] e [CONCEITO B].

Apresente:
- definição;
- objetivo;
- funcionamento;
- exemplo;
- quando usar;
- limitações.

Termine com uma síntese das principais diferenças.
```

### Preparação para prova

```text
Com base exclusivamente nas fontes selecionadas, crie 10 questões sobre [TEMA], misturando questões conceituais, situações práticas, verdadeiro ou falso e comparações.

Não mostre as respostas de imediato.

Depois das questões, apresente um gabarito comentado.
```

### Revisão crítica

```text
Analise a resposta anterior usando exclusivamente as fontes selecionadas.

Separe:
1. o que as fontes sustentam diretamente;
2. o que precisa de mais evidência;
3. o que não foi encontrado nas fontes;
4. possíveis ambiguidades.

Não acrescente informações externas.
```

---

## Conclusão

Este projeto mostrou que a IA pode ajudar no processo de aprendizagem quando é usada com critério: **boas fontes, perguntas bem feitas e revisão crítica das respostas**.

O processo também foi iterativo, porque só cheguei à versão final depois de testar, identificar problemas e corrigir as fontes e os arquivos utilizados.

A principal lição foi que a IA não substitui a participação do estudante. Ela funciona melhor como uma ferramenta de apoio para **pesquisar, organizar, questionar, revisar e consolidar o conhecimento**.

---

## Ferramentas utilizadas

* **NotebookLM** — organização das fontes, perguntas e revisão do conteúdo;
* **GitHub** — documentação e publicação do projeto;
* **Markdown** — estruturação do README;
* **Python** — ferramenta relacionada aos estudos de Ciência de Dados.
* **ChatGPT** — apoio na organização do projeto, elaboração e revisão de prompts e estruturação da documentação;
Claude — apoio na revisão e organização das informações do projeto;
