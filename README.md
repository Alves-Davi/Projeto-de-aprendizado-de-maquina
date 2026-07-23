# Detecção de URLs de Phishing com Aprendizado de Máquina

Projeto desenvolvido para a disciplina de **Fundamentos da inteligência artificial**, com o objetivo de comparar diferentes algoritmos de classificação na detecção de URLs de phishing.

## Integrantes

- Davi Alves Matos
- Nathan Alejandro Pereira Soarez Ramirez
- Rafael Gomes Bonfim Lédo

---

## Objetivo

Desenvolver e avaliar modelos de aprendizado de máquina capazes de classificar URLs como **legítimas** ou **maliciosas (phishing)** a partir de características extraídas das páginas e das próprias URLs.

Foram comparados diferentes algoritmos de classificação, utilizando métricas de desempenho para selecionar o modelo mais adequado.

---

## Dataset

**Nome:** PhiUSIIL Phishing URL (Website)

**Fonte:** UCI Machine Learning Repository

https://archive.ics.uci.edu/dataset/967/phiusiil+phishing+url+website

O conjunto de dados contém milhares de URLs acompanhadas por diversas características relacionadas ao domínio, conteúdo da página e propriedades da URL, além do atributo alvo (`label`), utilizado para indicar se uma URL é legítima ou de phishing.

---

## Tecnologias Utilizadas

- Python 3
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- UCI ML Repository (`ucimlrepo`)

---

## Como Executar

1. Abra o notebook no Google Colab.

2. Execute a célula responsável pela instalação da biblioteca:

```python
!pip install ucimlrepo
```

3. Execute todas as células do notebook na ordem em que aparecem.

O dataset será carregado automaticamente a partir do repositório oficial da UCI Machine Learning Repository.

---

## Etapas Desenvolvidas

- Compreensão dos Dados
- Análise Exploratória (EDA)
- Pré-processamento utilizando Pipeline
- Separação entre treino e teste
- Validação Cruzada
- Treinamento dos modelos
- Avaliação dos resultados
- Discussão dos resultados

---

## Modelos Avaliados

- DummyClassifier (Baseline)
- SGDClassifier
- Random Forest Classifier

---

## Métricas Utilizadas

- Acurácia
- Precisão
- Recall
- F1-Score
- Matriz de Confusão

---

## Resultados

Os modelos de aprendizado de máquina apresentaram desempenho significativamente superior ao modelo baseline.

| Modelo | Acurácia Média |
|---------|---------------:|
| Baseline | 57,19% |
| SGDClassifier | 99,98% |
| Random Forest | **99,99%** |

O Random Forest apresentou o melhor desempenho e foi selecionado como modelo final.

Na avaliação utilizando o conjunto de teste foram obtidos:

- **Acurácia:** 99,99%
- **Precisão:** 99,99%
- **Recall:** 99,99%
- **F1-Score:** 99,99%

A matriz de confusão mostrou apenas cinco classificações incorretas em mais de 47 mil exemplos avaliados.

---

## Principais Bibliotecas

```python
pandas
numpy
matplotlib
seaborn
scikit-learn
ucimlrepo
```

---

## Contribuição dos Integrantes

| Integrante | Atividades |
|------------|------------|
| Nathan Alejandro Pereira Soarez Ramirez | Compreensão dos dados e análise exploratória |
| Davi Alves Matos | Pré-processamento e treinamento dos modelos |
| Rafael Gomes Bonfim Lédo | Avaliação dos modelos e discussão dos resultados |

---

## Vídeo de Apresentação

Link para o vídeo:

**(Inserir link do vídeo aqui)**

---

## Uso de Inteligência Artificial

Durante o desenvolvimento deste projeto foi utilizada a ferramenta **ChatGPT** como apoio para:

- organização da estrutura do notebook;
- esclarecimento de dúvidas sobre a biblioteca Scikit-Learn;
- revisão do código;
- auxílio na documentação do projeto.

Todo o código, análises e resultados foram executados, revisados e validados pelos integrantes do grupo.

---

## Referências

- PRASAD, A.; CHANDRA, S. *PhiUSIIL Phishing URL Dataset*. UCI Machine Learning Repository, 2024.

- Pedregosa, F. et al. *Scikit-learn: Machine Learning in Python*. Journal of Machine Learning Research, 2011.

- Scikit-Learn Documentation: https://scikit-learn.org/
