# <h1 align="center"> Transfer-Learning-com-Python</h1>

Este repositório é referente a um projeto de Machine Learning com Transfer Learning para acelerar o aprendizado de um classificador de imagens para Gatos e Cachorros.
Para o projeto é utilizado o modelo pré-treinado InceptionV3 para classificar imagens de gatos e cachorros. Ele abrange desde a preparação do conjunto de dados até a visualização dos resultados do treinamento e testes em novas imagens.

## Funcionalidades

- **Download e Organização de Dados:** Realiza o download e organiza as imagens de treinamento, validação e teste.
- **Treinamento com InceptionV3:** Cria um modelo personalizado utilizando transfer learning com a base do InceptionV3.
- **Avaliação do Modelo:** Gera relatórios de classificação e matrizes de confusão para análise de desempenho.
- **Classificação de Novas Imagens:** Permite classificar novas imagens individuais ou em lote.
- **Visualização de Resultados:** Exibe curvas de aprendizado para avaliar o desempenho ao longo das épocas.

## Estrutura do Projeto

Exemplo de estrutura para o projeto.

```
├── dataset
│   ├── train
│   │   ├── cats
│   │   └── dogs
│   ├── val
│   │   ├── cats
│   │   └── dogs
│   └── test (opcional)
│       ├── cats
│       └── dogs
├── notebooks
│   └── Transfer_Learning_ML.ipynb
└── README.md
```

## Pré-requisitos

- Python 3.10 ou superior
- Bibliotecas Python: `tensorflow`, `numpy`, `matplotlib`, `scikit-learn`, `tqdm`

## Como Executar

> [!NOTE]
> Código executado no Google Colab. Caso queira executar em um máquina local poderá ser necessário modificações.

1. **Clone o Repositório:**

   ```bash
   git clone https://github.com/Danieltandrade/Transfer-Learning-com-Python.git
   ```

2. **Instale as Dependências:**

   ```bash
   pip install -r requirements.txt
   ```

3. **Execute o Notebook:**

   Abra o arquivo `Transfer_Learning_ML.ipynb` em um ambiente Jupyter ou Google Colab e siga os passos descritos.

## Testando Novas Imagens

Adicione as imagens a serem classificadas em uma pasta de sua escolha e utilize o código fornecido no notebook para carregá-las e classificá-las.

## Resultados

Nos testes o modelo se comportou de uma maneira bem satisfatória, com acurácia acima de 90%.
Abaixo segue exemplo dos dados apurado na execução do código:

- **Acurácia Média:** 96% no conjunto de validação
- **Exemplo de Matriz de Confusão:**

  ```
  [[46  4]
   [ 1 50]]
  ```

- **Curvas de aprendizado:** Gráficos exibindo acurácia e perda durante o treinamento.

## Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir uma issue ou enviar um pull request com melhorias e novas funcionalidades.

## Licença

Este projeto está licenciado sob a Licença GNU GENERAL PUBLIC LICENSE. Consulte o arquivo LICENSE para mais detalhes.

## Conclusão

O uso da técnica de Transfer Learning é uma grande ajuda em projeto de classificação de imagens, onde podemos utilizar diversos modelos disponíveis, reduzindo muito o tempo e o custo em relação a treinar um modelo do zero.
Este projeto pode ser ampliado para atender a necessidade de cada um, com vários parâmetros podendo ser alterados.
Também pode ser incluído um complemento de código para processar um novo conjunto de imagens e até a criação de uma API para ser colocado em produção.
Nos mais agradeço a todos.