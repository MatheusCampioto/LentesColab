# Classificação de Lentes de Contato

## Descrição

Este trabalho tem como objetivo aplicar o algoritmo Naive Bayes para classificar o tipo de lente de contato de um paciente, e comparar com uma Rede Bayesiana.

---

## Dados

O conjunto de dados possui 15 exemplos com os atributos:

* idade (infantil, adolescente, adulto)
* diagnostico (miopia, hipermetropia)
* astigmatismo (sim, nao)
* lacrimal (normal, reduzida)

Classe:

* lente (nenhuma, gelatinosa, dura)

---

## Método

Foi utilizado:

* Naive Bayes com suavização de Laplace (α = 1)
* Rede Bayesiana considerando que lacrimal depende da idade

---

## Paciente analisado

* idade: infantil
* diagnostico: hipermetropia
* astigmatismo: nao
* lacrimal: reduzida

---

## Resultados

Naive Bayes:

* nenhuma ≈ 0.457
* gelatinosa ≈ 0.467
* dura ≈ 0.075

Classe prevista: gelatinosa

Rede Bayesiana:

* nenhuma ≈ 0.413
* gelatinosa ≈ 0.422
* dura ≈ 0.164

Classe prevista: gelatinosa

---

## Conclusão

Os dois métodos classificaram o paciente como gelatinosa.
A rede bayesiana mudou um pouco as probabilidades, mas não alterou o resultado final.
