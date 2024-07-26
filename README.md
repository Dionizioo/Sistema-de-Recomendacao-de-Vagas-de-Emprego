# Sistema de Recomendação de Vagas de Emprego

Bem-vindo ao sistema de recomendação de vagas de emprego! Este projeto usa técnicas de Processamento de Linguagem Natural (NLP) e aprendizado de máquina para fornecer recomendações de empregos semelhantes com base na descrição do trabalho.

## Visão Geral

O objetivo deste projeto é ajudar candidatos a encontrar vagas de emprego que melhor se encaixem em seu perfil e preferências. Utilizamos um conjunto de dados de descrições de empregos e aplicamos técnicas de NLP para analisar e recomendar vagas.

## Funcionalidades

- **Carregamento e Visualização de Dados**: Importação de dados de descrições de vagas de emprego e visualização inicial.
- **Limpeza e Pré-processamento de Texto**: Limpeza de texto, tokenização, remoção de stopwords e stemming.
- **Análise Exploratória de Dados**: Visualização da distribuição do número de palavras em títulos e descrições de trabalho.
- **Vetorização usando TF-IDF**: Conversão de texto em vetores numéricos usando TF-IDF.
- **Cálculo de Similaridade**: Cálculo da similaridade coseno entre descrições de emprego.
- **Sistema de Recomendação**: Função para recomendar vagas de emprego semelhantes com base na descrição fornecida.
- **Visualização de Resultados**: Gráficos para análise das recomendações.

## Como Funciona

1. **Importação e Configuração do Ambiente**: Carregamos as bibliotecas necessárias e configuramos o ambiente.
2. **Download e Extração dos Dados**: Baixamos e extraímos os dados de descrições de vagas.
3. **Carregamento dos Dados**: Carregamos os dados em um DataFrame do Pandas e visualizamos as primeiras linhas.
4. **Limpeza e Pré-processamento**: Aplicamos técnicas de limpeza de texto para preparar os dados.
5. **Análise Exploratória**: Visualizamos a distribuição do número de palavras nos títulos e descrições de trabalho.
6. **Vetorização e Cálculo de Similaridade**: Vetorizamos o texto usando TF-IDF e calculamos a similaridade coseno.
7. **Recomendação de Vagas**: Implementamos uma função para recomendar vagas similares e testamos com exemplos.
8. **Salvar e Carregar Dados**: Salvamos os dados e modelos treinados para uso futuro.

## Exemplos de Uso

### Recomendação para um Título de Trabalho Existente

```python
# Testar a função de recomendação com um título de exemplo
print("\nRecomendações para 'medic front offic officeteam':")
print(recommendation('medic front offic officeteam'))
