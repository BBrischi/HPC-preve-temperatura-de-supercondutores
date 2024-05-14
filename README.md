<div>
        <img src="HPC LOGO.png" style="width: 500px; height:500px; margin-right: 20px;" />
</div>

# HPC preveem temperatura crítica de supercondutores
**Grupo:** HPC: High Phofocas & Condiments
<br>
**Integrantes:** Alice Barbarino Santos, Bruno Ferreira Brischi e Maria Eduarda de Oliveira Crist
<br>
**Instituição:** Ilum - Escola de ciência
<br>
## Apresentação
Este GitHub compõe um dos dois trabalhos finais de _Redes Neurais e Algoritmos Genéticos_, disciplina ministrada por Daniel Roberto Cassar na [Ilum - Escola de Ciências](https://ilum.cnpem.br). Dessa forma, esse projeto busca prever a temperatura crítica de supercondutores utilizando o dataset _Superconductivity Data_, feito por Kam Hamidieh. Então, para realizar as previsões, nos propomos a usar uma rede neural do tipo _perceptron_ multicamadas (MLP) e observar se é possível predizer de forma razoável a temperatura crítica de supercondutor

## Estrutura do Repositório
- _MLP supercondutora.ipynb_: Jupyter Notebook que apresenta a rede neural, bem como todo o seu processo de treinamento, teste e tratamento de dados;
- _train.csv_: csv que possui o dataset usado para o treinamento da rede neural.

## Motivação
O fenômeno da supercondutividade foi descoberta pela primeira vez em 1911, pelo físico holândes Heike Kamerlingh Onnes, que ganhou um Nobel de Física para sua descoberta, em 1913. Um material se caracteriza como supercondutor se, abaixo de uma determinada temperatura, chamada de Temperatura crítica ($T_c$), ele não apresentar resistência elétrica e gerar campos magnéticos. Devido à essas propriedades únicas, os supercondutores vêm sendo extensivamente pesquisados desde então pelas suas possibilidades de aplicação em diversas áreas [[1]](https://home.cern/science/engineering/superconductivity) [[2]](https://www.inmesol.com/blog/superconductivity-applied-to-everyday-life/#:~:text=Superconductivity%20is%20the%20ability%20of,are%20some%20applications%20of%20superconductivity). Ainda assim, não possuímos uma teoria que realmente explique o porquê de os supercondutores apresentarem essas propriedades, o que dificulta a previsão de quais materiais podem ser supercondutores e qual a temperatura crítica desses materiais. Por isso, um trabalho que se proponha a predizer essas temperaturas críticas desses materiais pode ser muito útil para dar _insights_ sobre a teoria por trás dos supercondutores.

## Requisitos
É necessário o python instalado, além do Jupyter habilitado com as bibliotecas: `pandas`, `torch`, `optuna`, `sklearn`, `lightning`, `matplotlib`, `numpy`, `scipy` e `random`, que são usadas em momentos variados do código.

## Bibliotecas
_Listar quais são as bibliotecas utilizadas, suas funções e qual foi seu uso no trabalho_
As principais bibliotecas utilizadas nesse trabalho são: 
- `pandas` para tratamento de dados, `sklearn` para normalização e _split_ dos dados;
- `torch` e `lighting` para a construção da rede neural;
- `optuna` para otimização dos hiperparâmetros da MLP;
Além do uso ocasional de `matplotlib` para representação gráfica e uso adicional das bibliotecas `numpy`, `scipy` e `random` como suporte em alguma tarefa específica.

## Como utilizar
Nesse repositório, o usuário tem acesso à um notebook executável, que pode ser baixado e executado pelo usuário, com o intuito de que ele entenda passo a passo da construção e treino da rede neural, além de apresentar dados sobre sua performance. Por já apresentar a rede neural treinada, o usuário pode usufruir desse notebook para fazer previsões por si só, desfrutando do modelo apresentado.
Obs.: o notebook foi executado em um Lenovo ThinkPad E14 i5, demorando cerca de 8 horas para sua execução completa; devido ao fato de ser um código pesado, recomendamos seu uso em uma máquina com um bom processador.

## Referências
<ul>
    <li><a href="https://home.cern/science/engineering/superconductivity">Superconductivity - CERN</a></li>
    <li><a href="https://www.inmesol.com/blog/superconductivity-applied-to-everyday-life/#:~:text=Superconductivity%20is%20the%20ability%20of,are%20some%20applications%20of%20superconductivity.">Superconductivity Applied to Everyday Life - Inmesol</a></li>
    <li><a href="https://www.semanticscholar.org/paper/A-data-driven-statistical-model-for-predicting-the-Hamidieh/b3bea0ac481f0869cb746f3b44d5689bf1a9b924">A data-driven statistical model for predicting the - Semantic Scholar</a></li>
    <li><a href="https://www.analyticsvidhya.com/blog/2023/11/train-test-validation-split/">A comprehensive guide to train-test-split - Analytics Vidhya</a></li>
    <li><a href="https://medium.com/ipnet-growth-partner/padronizacao-normalizacao-dados-machine-learning-f8f29246c12">Padronização e Normalização de Dados em Machine Learning - Medium</a></li>
    <li><a href="https://lightning.ai/docs/pytorch/stable/data/datamodule.html">DataModule - Lightning</a></li>
    <li>Notebook sobre lightning (material da disciplina disponibilizado pelo professor)</li>
    <li><a href="https://www.youtube.com/watch?v=VMj-3S1tku0&list=PLAqhIrjkxbuWI23v9cThsA9GvCAUhRvKZ">Vídeo sobre Lightning - YouTube</a></li>
    <li><a href="https://dl.acm.org/doi/10.1145/3292500.3330701">Hyper-Parameter Optimization - ACM Digital Library</a></li>
    <li>Notebook sobre normalização (material disponibilizado pelo professor)</li>
    <li>Notebook sobre sklearn (material da disciplina disponibilizado pelo professor)</li>
    <li><a href="https://medium.com/ensina-ai/rede-neural-perceptron-multicamadas-f9de8471f1a9">Rede Neural Perceptron Multicamadas - Medium</a></li>
    <li><a href="https://pytorch.org/docs/stable/optim.html">Optim Module - PyTorch</a></li>
    <li><a href="https://pytorch.org/docs/stable/generated/torch.nn.Tanh.html">torch.nn.Tanh - PyTorch</a></li>
    <li><a href="https://wandb.ai/authors/ayusht/reports/Implementing-Dropout-Regularization-in-PyTorch--VmlldzoxNTgwOTE">Implementing Dropout Regularization in PyTorch - Weights & Biases</a></li>
    <li><a href="https://optuna.org/#code_examples">Optuna Examples - Optuna</a></li>
    <li><a href="https://towardsdatascience.com/https-medium-com-perlitz-hyper-parameter-optimization-with-optuna-1c32785e7df">Hyper Parameter Optimization with Optuna - Towards Data Science</a></li>
    <li><a href="https://towardsdatascience.com/simple-guide-to-hyperparameter-tuning-in-neural-networks-3fe03dad8594">Simple Guide to Hyperparameter Tuning in Neural Networks - Towards Data Science</a></li>
    <li><a href="https://lightning.ai/docs/pytorch/stable/common/early_stopping.html">Early Stopping - Lightning</a></li>
    <li><a href="https://pytorch.org/docs/stable/generated/torch.nn.Dropout.html">torch.nn.Dropout - PyTorch</a></li>
    <li><a href="https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.MaxAbsScaler.html">MaxAbsScaler - Scikit-Learn</a></li>
</ul>
