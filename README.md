# SafeConnect: Previsão Inteligente de Doenças com Dados Reais

---

## Índice

- [Introdução](#introdução)
- [Objetivo do Projeto](#objetivo-do-projeto)
- [Pitch Resumido](#pitch-resumido)
- [Tecnologias e Conceitos Utilizados](#tecnologias-e-conceitos-utilizados)
- [Fontes de Dados](#fontes-de-dados)
- [Como Utilizar](#como-utilizar)
  - [Pré-requisitos](#pré-requisitos)
  - [Instalação](#instalação)
  - [Execução](#execução)
- [Resultados Obtidos](#resultados-obtidos)
- [Possíveis Melhorias](#possíveis-melhorias)
- [Contribuições](#contribuições)
- [Licença](#licença)
- [Agradecimentos](#agradecimentos)

---

## Introdução

O **SafeConnect** é uma plataforma inovadora que utiliza dados reais e técnicas avançadas de inteligência artificial para prever a disseminação de doenças em escala global. Este projeto foi desenvolvido como parte da **Pós-Graduação em Data Science da Faculdade Descomplica**, no contexto do **Módulo 03**, que aborda temas como Regressão e Predição, Deep Learning, Network Science, Perceptron e Adaline.

---

## Objetivo do Projeto

- **Prever a propagação de doenças** utilizando dados reais e modelos de inteligência artificial.
- **Auxiliar autoridades de saúde** na tomada de decisões estratégicas e alocação de recursos.
- **Demonstrar a aplicação prática** das disciplinas do Módulo 03 em um projeto integrado.

---

## Pitch Resumido

A rápida propagação de doenças, como a COVID-19, evidencia a necessidade de ferramentas preditivas eficazes. O SafeConnect utiliza dados reais de fontes confiáveis, integrados com técnicas avançadas de inteligência artificial, para prever a disseminação de doenças e auxiliar na tomada de decisões estratégicas. Com isso, buscamos capacitar governos e comunidades a agir de forma eficaz, salvando vidas e recursos.

---

## Tecnologias e Conceitos Utilizados

1. **Regressão e Predição**
   - Modelo **Random Forest Regressor** para prever o logaritmo do número de novos casos com base em dados de população e casos confirmados.
2. **Deep Learning**
   - Implementação de **Redes Neurais Artificiais (MLPClassifier)** com ajuste de hiperparâmetros e validação cruzada estratificada para classificação de países com alto risco de aumento de casos.
3. **Perceptron e Adaline**
   - Embora não utilizados na versão final devido a ajustes para melhorar o desempenho, os conceitos foram considerados no desenvolvimento inicial.
4. **Network Science**
   - Análise de centralidade dos países em uma rede global simplificada para entender sua influência na propagação de doenças.
5. **Validação Cruzada e Ajuste de Hiperparâmetros**
   - Uso de **Stratified K-Fold Cross-Validation** e **GridSearchCV** para garantir a generalização dos modelos e evitar overfitting.

---

## Fontes de Dados

- **Casos Confirmados de COVID-19**
  - Fonte: [Johns Hopkins University Center for Systems Science and Engineering (JHU CSSE)](https://github.com/CSSEGISandData/COVID-19)
  - URL: `https://github.com/CSSEGISandData/COVID-19`
- **Dados Demográficos**
  - Fonte: [World Bank Open Data](https://data.worldbank.org/)
  - URL: `https://data.worldbank.org/indicator/SP.POP.TOTL`

---

## Como Utilizar

### Pré-requisitos

- **Python 3.7+**
- Bibliotecas Python:
  - `numpy`
  - `pandas`
  - `networkx`
  - `matplotlib`
  - `requests`
  - `scikit-learn`
  - `seaborn`

### Instalação

1. **Clone o repositório**

   ```bash
   git clone https://github.com/seu-usuario/safeconnect.git
   ```

2. **Navegue até o diretório do projeto**

   ```bash
   cd safeconnect
   ```

3. **Crie um ambiente virtual (opcional, mas recomendado)**

   ```bash
   python -m venv venv
   source venv/bin/activate  # Linux/Mac
   venv\Scripts\activate  # Windows
   ```

4. **Instale as dependências**

   ```bash
   pip install -r requirements.txt
   ```

### Execução

1. **Execute o script principal**

   ```bash
   python safeconnect.py
   ```

2. **Visualize os resultados**

   - Os gráficos e resultados serão exibidos na tela.
   - Logs e métricas serão exibidos no console.

---

## Resultados Obtidos

- **Random Forest Regressor**
  - *MSE (Erro Médio Quadrático)*: 6.56
  - *Interpretação*: O modelo consegue prever com boa precisão o logaritmo do número de novos casos.

- **Random Forest Classifier**
  - *Acurácia no conjunto de teste*: 100%
  - *Acurácia média na validação cruzada estratificada*: 100%
  - *Interpretação*: O modelo é altamente eficaz na classificação de países com alto risco de aumento de casos. A validação cruzada indica excelente capacidade de generalização.

- **MLPClassifier (Rede Neural Artificial)**
  - *Acurácia no conjunto de teste*: 100%
  - *Acurácia média na validação cruzada estratificada*: 100%
  - *Interpretação*: Após ajuste de hiperparâmetros e aplicação de técnicas para evitar overfitting, o modelo apresenta desempenho excepcional.

- **Análise de Network Science**
  - A inclusão da centralidade dos países como variável preditora contribuiu para melhorar o desempenho dos modelos.

---

## Possíveis Melhorias

- **Análise de Overfitting**
  - Apesar das altas acurácias, é importante continuar monitorando para evitar sobreajuste, especialmente com dados futuros.

- **Dados Adicionais**
  - Incorporar variáveis como índices de mobilidade, medidas governamentais e taxas de vacinação para enriquecer os modelos.

- **Modelos Avançados**
  - Explorar modelos de séries temporais ou redes neurais recorrentes (LSTM) para capturar dependências temporais.

- **Refinamento da Rede**
  - Utilizar dados reais de conexões entre países (fluxos de viagens, fronteiras) para aprimorar a análise de network science.

---

## Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir *issues* e enviar *pull requests*.

1. **Fork o repositório**
2. **Crie uma nova branch**

   ```bash
   git checkout -b feature/nova-funcionalidade
   ```

3. **Commit suas alterações**

   ```bash
   git commit -m "Descrição da nova funcionalidade"
   ```

4. **Envie para o repositório remoto**

   ```bash
   git push origin feature/nova-funcionalidade
   ```

5. **Abra um Pull Request**

---

## Licença

Este projeto está licenciado sob a [MIT License](LICENSE).

---

## Agradecimentos

- **Faculdade Descomplica**
  - Pela oportunidade de aplicar conhecimentos adquiridos na **Pós-Graduação em Data Science**.
- **Professores e Colegas**
  - Pelo suporte e feedback durante o desenvolvimento do projeto.
- **Comunidade Open Source**
  - Pelas bibliotecas e datasets disponibilizados, fundamentais para este projeto.

---

**Contato:** [seu.email@dominio.com](mailto:seu.email@dominio.com)

---

*Este projeto é parte dos requisitos do Módulo 03 da Pós-Graduação em Data Science da Faculdade Descomplica.*