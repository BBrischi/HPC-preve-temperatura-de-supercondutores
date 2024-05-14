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
_Colocar TODAS e QUALQUER referência que a gente venha usar._
[1]https://home.cern/science/engineering/superconductivity
[2] https://www.inmesol.com/blog/superconductivity-applied-to-everyday-life/#:~:text=Superconductivity%20is%20the%20ability%20of,are%20some%20applications%20of%20superconductivity
[3] artigo do amg
