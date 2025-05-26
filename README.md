# Reconhecimento de Imagens com Redes Neurais Convolucionais (CNNs)

As CNNs são um tipo especial de rede neural projetada para **análise de dados visuais**. Ao contrário das redes tradicionais, as CNNs utilizam **camadas convolucionais** que operam como filtros, extraindo características relevantes das imagens (bordas, texturas, formas, etc.).

### Por que CNNs são eficientes?

- Capturam **padrões espaciais locais** através de filtros (kernels)
- Reduzem a dimensionalidade com **camadas de pooling**
- Possuem **parâmetros compartilhados**, o que reduz a complexidade e acelera o treinamento
- São especialmente eficazes em tarefas como **reconhecimento de imagens, detecção de objetos, e visão computacional**

### Exemplo intuitivo

Imagine que temos uma imagem de um número “8”. A CNN começa detectando **linhas horizontais**, depois **curvas** e **intersecções**, até finalmente classificar como o dígito **8** com base nos padrões aprendidos.

---

## 📂 Estrutura dos Notebooks

### 1. `CNN1_CIFAR10_Orlando.ipynb`
**📌 Tarefa:** Classificação de 10 categorias de imagens coloridas (avião, carro, pássaro, gato, etc.)  
**📚 Dataset:** [CIFAR-10](https://www.cs.toronto.edu/~kriz/cifar.html)  
**🔍 Destaques:**
- Pré-processamento de imagens RGB
- Arquitetura de CNN com múltiplas camadas convolucionais e pooling
- Avaliação de acurácia por classe

### 2. `CNN2_Identificacao_Digitos_Orlando.ipynb`
**📌 Tarefa:** Reconhecimento de dígitos manuscritos  
**📚 Dataset:** [MNIST](http://yann.lecun.com/exdb/mnist/)  
**🔍 Destaques:**
- Conversão de escala de cinza
- Otimização da arquitetura para alta acurácia
- Análise visual de previsões corretas e incorretas

### 3. `CNN3_Identificacao_Gatos_Cachorros_Orlando.ipynb`
**📌 Tarefa:** Classificação binária entre gatos e cachorros  
**📚 Dataset:** [Dogs vs. Cats (Kaggle)](https://www.kaggle.com/c/dogs-vs-cats)  
**🔍 Destaques:**
- Aplicação de **data augmentation**
- Uso de camadas de dropout para prevenir overfitting
- Visualização de filtros aprendidos pela rede

### 4. `CNN4_Identificacao_Personagens_Orlando.ipynb`
**📌 Tarefa:** Classificação de personagens específicos (dataset personalizado ou animado)  
**📚 Dataset:** Imagens personalizadas (informar origem)  
**🔍 Destaques:**
- Treinamento com conjunto de dados customizado
- Análise de performance por personagem
- Uso de `ImageDataGenerator` para preparação de dados

---

## 📈 Métricas de Avaliação

As CNNs foram avaliadas com as métricas de:

- **Acurácia**
- **Loss (função de custo)**
- **Matriz de confusão**
- **Visualizações das classificações corretas/incorretas**
