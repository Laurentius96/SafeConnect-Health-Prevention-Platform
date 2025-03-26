Aqui está o README.md atualizado com a licença CC BY-NC-ND 4.0 em substituição à licença MIT:

# SafeConnect | Intelligent Disease Prevention Platform Using Real-World Data
---

## Table of Contents

- [Introduction](#introduction)
- [Project Objective](#project-objective)
- [Executive Summary](#executive-summary)
- [Technologies and Concepts](#technologies-and-concepts)
- [Data Sources](#data-sources)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Running the Application](#running-the-application)
- [Results](#results)
- [Future Improvements](#future-improvements)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

---

## Introduction

**SafeConnect** is an innovative platform that leverages real-world data and advanced AI techniques to predict disease spread on a global scale. This project was developed as part of the **Data Science Post-Graduate Program at Descomplica College**, specifically for **Module 03**, which covers Regression and Prediction, Deep Learning, Network Science, Perceptron, and Adaline.

---

## Project Objective

- **Predict disease spread** using real-world data and AI models
- **Support health authorities** in strategic decision-making and resource allocation
- **Demonstrate practical application** of Module 03 concepts in an integrated project

---

## Executive Summary

The rapid spread of diseases like COVID-19 highlights the critical need for effective predictive tools. SafeConnect combines reliable real-world data with advanced AI techniques to forecast disease spread and support strategic decision-making. Our platform empowers governments and communities to take effective action, ultimately saving lives and resources.

---

## Technologies and Concepts

1. **Regression and Prediction**
   - **Random Forest Regressor** model for predicting the logarithm of new cases based on population and confirmed case data
2. **Deep Learning**
   - Implementation of **Artificial Neural Networks (MLPClassifier)** with hyperparameter tuning and stratified cross-validation for high-risk country classification
3. **Perceptron and Adaline**
   - While not used in the final version due to performance optimization, these concepts influenced early development
4. **Network Science**
   - Country centrality analysis in a simplified global network to understand disease spread influence
5. **Cross-Validation and Hyperparameter Tuning**
   - Utilizing **Stratified K-Fold Cross-Validation** and **GridSearchCV** to ensure model generalization and prevent overfitting

---

## Data Sources

- **COVID-19 Confirmed Cases**
  - Source: [Johns Hopkins University Center for Systems Science and Engineering (JHU CSSE)](https://github.com/CSSEGISandData/COVID-19)
  - URL: `https://github.com/CSSEGISandData/COVID-19`
- **Demographic Data**
  - Source: [World Bank Open Data](https://data.worldbank.org/)
  - URL: `https://data.worldbank.org/indicator/SP.POP.TOTL`

---

## Getting Started

### Prerequisites

- **Python 3.7+**
- Required Python libraries:
  - `numpy`
  - `pandas`
  - `networkx`
  - `matplotlib`
  - `requests`
  - `scikit-learn`
  - `seaborn`

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/your-username/safeconnect.git
   ```

2. **Navigate to project directory**

   ```bash
   cd safeconnect
   ```

3. **Create virtual environment (recommended)**

   ```bash
   python -m venv venv
   source venv/bin/activate  # Linux/Mac
   venv\Scripts\activate  # Windows
   ```

4. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

### Running the Application

1. **Run the main script**

   ```bash
   python safeconnect.py
   ```

2. **View results**
   - Graphs and results will display on screen
   - Logs and metrics will appear in console

---

## Results

- **Random Forest Regressor**
  - *Mean Squared Error*: 6.56
  - *Interpretation*: Model accurately predicts the logarithm of new cases

- **Random Forest Classifier**
  - *Test Set Accuracy*: 100%
  - *Stratified Cross-Validation Mean Accuracy*: 100%
  - *Interpretation*: Highly effective in classifying high-risk countries with excellent generalization capability

- **MLPClassifier (Neural Network)**
  - *Test Set Accuracy*: 100%
  - *Stratified Cross-Validation Mean Accuracy*: 100%
  - *Interpretation*: Exceptional performance after hyperparameter tuning and overfitting prevention

- **Network Science Analysis**
  - Country centrality as a predictor variable improved model performance

---

## Future Improvements

- **Overfitting Analysis**
  - Continue monitoring high accuracy rates to prevent overfitting with future data

- **Additional Data**
  - Incorporate mobility indices, government measures, and vaccination rates

- **Advanced Models**
  - Explore time series models or LSTM networks for temporal dependencies

- **Network Refinement**
  - Use actual country connection data (travel flows, borders) to enhance network science analysis

---

## Contributing

Contributions are welcome! Feel free to open issues and submit pull requests.

1. **Fork the repository**
2. **Create a feature branch**

   ```bash
   git checkout -b feature/new-feature
   ```

3. **Commit changes**

   ```bash
   git commit -m "Feature description"
   ```

4. **Push to remote**

   ```bash
   git push origin feature/new-feature
   ```

5. **Open a Pull Request**

---

## License

This project is licensed under the Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License (CC BY-NC-ND 4.0). See the [LICENSE](LICENSE.md) file for details.

### What this means:

- **Attribution required** — You must give appropriate credit, provide a link to the license, and indicate if changes were made
- **NonCommercial** — You may not use the material for commercial purposes
- **NoDerivatives** — If you remix, transform, or build upon the material, you may not distribute the modified material
- **No additional restrictions** — You may not apply legal terms or technological measures that legally restrict others from doing anything the license permits

For the complete CC BY-NC-ND 4.0 license terms, please refer to the [LICENSE](LICENSE.md) file in this repository or visit [Creative Commons](https://creativecommons.org/licenses/by-nc-nd/4.0/).

---

## Acknowledgments

- **Descomplica College**
  - For the opportunity to apply knowledge gained in the **Data Science Post-Graduate Program**
- **Open Source Community**
  - For providing essential libraries and datasets

---

**Contact:** 

For questions or suggestions about this repository, please contact me through GitHub.

---

*This project fulfills requirements for Module 03 of the Data Science Post-Graduate Program at Descomplica College.*
