# Inteligência Artificial: Previsão de Score de Crédito 🧠💳

Este projeto utiliza Machine Learning para automatizar a análise de perfil de crédito de clientes. O objetivo é classificar novos clientes em três categorias de score (Good, Standard, Poor), auxiliando instituições financeiras na tomada de decisão sobre concessão de crédito.

## 📁 Estrutura de Arquivos
- `main.ipynb`: Jupyter Notebook com todo o pipeline de dados (limpeza, codificação e treinamento).
- `clientes.csv`: Base de dados histórica usada para o treinamento dos modelos.
- `novos_clientes.csv`: Base de dados de novos clientes usada para realizar as previsões finais.

## 🛠️ Tecnologias e Bibliotecas
- **Python 3**
- **Pandas**: Para manipulação e análise exploratória de dados.
- **Scikit-Learn (Sklearn)**: Para a implementação dos algoritmos de Machine Learning e métricas de avaliação.

## 🤖 Fluxo de Desenvolvimento
1. **Pré-processamento (Data Cleaning)**: Identificação e tratamento de colunas não numéricas que precisam ser convertidas para que a IA processe a informação.
2. **Label Encoding**: Uso do `LabelEncoder` para transformar categorias (como Profissão e Mix de Crédito) em valores numéricos.
3. **Divisão de Dados**: Separação da base em conjuntos de **Treino** (80%) e **Teste** (20%).
4. **Treinamento de Modelos**: Foram treinados dois algoritmos principais:
   - **Random Forest (Árvore de Decisão)**
   - **KNN (K-Nearest Neighbors)**
5. **Avaliação**: Comparação da acurácia de cada modelo para definir o mais eficaz.



## 📊 Performance dos Modelos
Após os testes, o modelo de **Random Forest** demonstrou maior precisão na classificação dos perfis de crédito, sendo escolhido para realizar as previsões na base de `novos_clientes.csv`.

## ⚙️ Como Executar
1. Certifique-se de ter as bases `.csv` na mesma pasta do código.
2. Instale as dependências:
   ```bash
   pip install pandas scikit-learn
3. Execute o arquivo main.ipynb utilizando Jupyter ou VS Code.
Projeto desenvolvido durante a Jornada Python da Hashtag Treinamentos.
