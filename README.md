# 🐧 Análise Exploratória de Dados: Palmer Penguins

Trabalho prático individual desenvolvido para a disciplina de **Princípios de Ciência de Dados** na **FATEC Cotia** (Data: 28/09/2026).

O objetivo deste projeto foi conduzir uma análise exploratória de dados (EDA) completa utilizando o clássico dataset **Palmer Penguins**, aplicando técnicas de manipulação de dados, tratamento de valores ausentes e visualização estatística em Python.

## 🛠️ Tecnologias e Ferramentas
* **Ambiente:** Google Colab
* **Linguagem:** Python
* **Bibliotecas:** Pandas, Matplotlib, Seaborn
* **Suporte de IA:** Utilização de prompts estruturados junto ao Gemini no Colab para auxiliar na escrita e validação dos códigos, mantendo o rigor analítico humano na definição de perguntas, limites e interpretações.

## 📊 Etapas da Análise e Principais Questões

### 1. Conhecimento e Limpeza da Base de Dados
* **Volume:** O dataset original contém **344 registros** (linhas) e **7 variáveis** (colunas).
* **Tratamento de Ausências:** Identificação e mapeamento de valores ausentes (`NaN`) em colunas anatômicas e de sexo, garantindo que os registros incompletos fossem filtrados adequadamente apenas nas análises correspondentes sem descartar dados desnecessariamente.

### 2. Q1: Contagem de Registros por Espécie
* **Análise:** Investigação da composição do dataset entre as três espécies disponíveis (*Adelie*, *Chinstrap* e *Gentoo*).
* **Visualização:** Geração de um gráfico de barras, evidenciando a distribuição dos 344 registros válidos (com destaque para a espécie *Adelie* como a mais frequente, com 152 registros).

### 3. Q2: Distribuição da Massa Corporal entre as Espécies
* **Análise:** Comparação das medidas descritivas (mínimo, quartis, mediana, máximo e média) da massa corporal (`body_mass_g`) agrupadas por espécie, utilizando 342 registros válidos.
* **Visualização:** Construção de um **Boxplot** que revelou visualmente a forte sobreposição de peso entre as espécies *Adelie* e *Chinstrap* (ambas com mediana de 3700 g) e a discrepância dos pinguins *Gentoo*, que se mostraram significativamente mais pesados (mediana de 5000 g), além de identificar *outliers* isolados.

### 4. Q3: Relação entre Comprimento da Nadadeira e Massa Corporal
* **Análise:** Investigação conjunta de pares de variáveis do mesmo indivíduo (`flipper_length_mm` e `body_mass_g`) em 342 registros válidos.
* **Visualização:** Criação de um **Gráfico de Dispersão (Scatter Plot)** com distinção de cores por espécie, permitindo observar a tendência positiva de que pinguins com nadadeiras mais compridas tendem a apresentar maior massa corporal, com os *Gentoo* posicionados no extremo superior da distribuição.

## 🔍 Limitações Analíticas
Ressalta-se que a análise exploratória descreve padrões amostrais e associações observadas, mas **não comprova relações de causalidade** (por exemplo, o gráfico de dispersão mostra que as medidas andam juntas, mas não prova que o tamanho da nadadeira seja a causa direta da variação de peso).

## 🚀 Como Visualizar
Você pode explorar o código executável completo, os blocos de manipulação em Pandas e a geração dos gráficos interativos abrindo o arquivo **`EDA_João_Alvarino.ipynb`** diretamente neste repositório ou no Google Colab!
