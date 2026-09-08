# Dostoiévski vs. Tolstói: Classificação de Autoria por Tema, Não por Estilo

## Objetivo

Investigar se é possível identificar o autor de um trecho de texto — Fiódor Dostoiévski ou Liev Tolstói — baseando-se **apenas em conteúdo temático** (do que o texto fala), e não em características estilométricas de superfície (tamanho de frase, pontuação, vocabulário raro, etc).

A hipótese central é que os dois autores têm "impressões digitais temáticas" distintas, mesmo escrevendo no mesmo período, no mesmo idioma original e no mesmo gênero (romance realista russo do século XIX):

- **Dostoiévski**: culpa, fé, crime, psicologia extrema, sofrimento individual
- **Tolstói**: sociedade, família, história, moralidade cotidiana

O projeto usa **topic modeling** e **embeddings semânticos** (via `sentence-transformers`) como features de classificação, isolando sinal temático de sinal estilístico — se um classificador ainda consegue prever o autor corretamente usando só essas features, isso é evidência de que o tema por si só já distingue os autores.

## Corpus

Textos em inglês, obtidos do [Project Gutenberg](https://www.gutenberg.org/) (domínio público).

*(lista de obras a ser definida)*

## Metodologia

1. Coleta e limpeza dos textos
2. Segmentação em trechos comparáveis
3. Topic modeling (LDA / NMF)
4. Embeddings semânticos (`sentence-transformers`)
5. Classificação de autoria usando apenas features temáticas
6. Avaliação e análise dos resultados

## Estrutura do repositório
