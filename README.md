# Analise-de-Aprendizado-Semi-supervisionado

**Trabalho 1 da Disciplina de Aprendizado de Máquina 2**

**Professor: Diego Furtado Silva**

Integrantes:

- Lucas Vinícius Domingues 769699

- Rafael Yoshio Yamawaki Murata 769681

- Victor Luís Aguilar Antunes 769734


## Links para os datasets: ##

- [ada_prior](https://www.openml.org/d/1037): Dataset de classificação para a tarefa de encontrar indivíduos com alta renda
- [ilpd](https://www.openml.org/d/1480): Pacientes hepáticos e não hepáticos na Índia
- [biomed](https://www.openml.org/d/481): Dataset para a tarefa de identificação de indivíduos portadores de uma condição genética rara
- [Qualitative Bankruptcy](https://archive.ics.uci.edu/ml/datasets/Qualitative_Bankruptcy): Dataset com dados parâmetros de empresas coletados por especialistas com o intuito de detectar empresas que foram à falência
- [irish](https://www.openml.org/d/451): Dataset com dados da educação irlandesa a respeito 500 alunos com 11 anos em 1967, com o objetivo de identificar se o exame final foi foi prestado pela criança ou não

> A análise utilizou 3 algorítimos de aprendizado supervisionado: Label Propagation, Label Spreading e Self Training, todos disponíveis na biblioteca scikit-learn.

> Para a avaliação dos algorítimos, foram retirados 64% das labels de cada dataset. Então, é feita a imputação destes valores pelos 3 algorítimos de aprendendizado semi-supervisionado mencionados.
Em seguida, os dados imputados são passados como conjunto de treinamento para classificadores SVM.

> Esses classificadores SVMs treinados com rótulos imputados são comparados com um classificador SVM que utilizou somente 36% do conjunto total de dados, ou seja, somente os dados que não tiveram seus rótulos retirados e posteriormente imputados. O intuito dessa comparação é verificar a aplicabilidade dos algorítimos de aprendizado semi-supervisionado na situação de falta de dados de cada um dos 5 datasets escolhidos.
