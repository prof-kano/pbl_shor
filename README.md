## Introdução
Este repositório contém os materiais necessários para a execução da atividade prática do dia 11/12/2024 da disciplina optativa de Quantum Safe do Instituto de Tecnologia e Liderança (Inteli).

Nesse laboratório aprenderemos como o Algoritmo de Shor 


## Requisitos

### • Instalação - Qiskit
<p align="justify">
A biblioteca Qiskit, um projeto da IBM, é uma das soluções adotadas para o desenvolvimento das atividades dessa disciplina.

Para isso, crie uma conta na IBM Quantum Platform (https://quantum.ibm.com/). Instale a biblioteca seguindo os passos do seguinte link oficial (https://docs.quantum.ibm.com/guides/install-qiskit), ou, seguindo este vídeo (https://www.youtube.com/watch?v=dZWz4Gs_BuI). Você poderá simular a execução de algoritmos quânticos na sua própria máquina ou submetê-los para execução nos computadores quânticos disponibilizados pela IBM (para isso utilize o token de API disponibilizado na sua conta). Have fun!
</p>

### • Instalação - PyCryptoDome

Instale a biblioteca de criptografia através da linha da seguinte comando pip no seu ambiente:

```
pip install pycryptodome
```

## Ideia Principal do Ataque 

O módulo público _n_ é igual a um número primo _p_ vezes um número primo _q_. Se você conhece _p_ e _q_ (e _e_ da chave pública), poderá determinar a chave privada, quebrando assim a criptografia. No entanto, fatorar um _n_ grande é muito difícil sem o uso de um computador quântico potente. Um _n_ pequeno, talvez, possa ser fatorado através do Algoritmo de Shor em um computador quântico disponível agora. Vamos descobrir! 

Quebrando _n_, cada grupo poderá derivar a chave privada (_d_) dos outros grupos com _p_, _q_, e _e_ através da seguinte relação _d ≡ e^-1 mod Φ(n)_.

## Fluxo da Dinâmica
![alice bob carlos drawio](https://github.com/user-attachments/assets/b656db96-39d7-4428-859f-ce014e5995da)

### • Canal de Comunicação Simulado
Iremos utilizar um drive aberto para que cada grupo disponibilize os dados considerados públicos em uma comunicação:
#### https://drive.google.com/drive/folders/15dsGyEeDWbrR268lTc6S-Et531BGVeLy?usp=sharing
Crie uma pasta com o nome do seu grupo e dentro dela sube a pasta "public" resultante da execucação do programa "Alice_Bob". 
Acesse e copie a pasta "public" disponibilizada por cada grupo. 
