# PWBE-Formativo 

## Passo a Passo para rodar o meu Projeto 🏃‍♀️

Este projeto Formativo foi proposto pelo Senai Roberto Mange, na disciplina de PWBE. Esse projeto é uma API para fazer o gerenciamento de um sistema escolar. Esse sistema permite que o Gestor possa fazer o gerenciamento de salas, reserva de ambientes, disciplinas e usuarios.

- Quer saber como faz para rodar esse Projeto 🤔
  
- siga o passo a passo 👣

# O que você precisa ter em seu computador?
 - VSCODE instalado;
 - Python instalado;
 - MYSQL;
   
❗É essencial que você tenha eles instalados

***

## 1- Clonar Repositório 📂

- Clicar no Botão azul escrito 'CODE'
- Copiar esse link: 'https://github.com/luanaGrandi/PWBE-Formativo.git'
- Escrever no CMD: git clone https://github.com/luanaGrandi/PWBE-Formativo.git

Após isso o meu repositorio já está em sua máquina 🥳

- Abri a pasta no VSCODE

## 2- Criar ambiente virtual ⚙️
  - Abrir o terminal o VSCODE
  - Criar ambiente virtual: ```python -m venv env```
  - Ativar o ambiente virtual: ```.\venv\Scripts\activate```

## 3- Instalar as dependências 🛠️
  - Instalar: ```pip install -r requirements.txt```

## 4- Verificar banco de dados 🔍

Nesse projeto estamos utilizando o banco de dados, para que ele funcione sem nenhume erro, faça essas passos:
 - entre na pasta: projeto;
 - entre no: ```settings.py```
 - procure o nome:```DATABASES```
- Veja se ele está correto desta forma:
  ```
   'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'cadastro',
        'USER': 'root',
        'PASSWORD': 'senai', -> essa senha será de acordo com a senha do seu mysql
        'HOST': 'localhost',
        'PORT': '3306'
    }
  ```


Para que o banco de dados funcione, você precisa criar a tabela no MySQL Workbench, usando o comando

```CREATE DATABASE cadastro (nome da tabela)```

Após a criação da tabela no banco de dados. De esses comandos para salvar suas alterações:
 ```py manage.py makemigrations
    py manage.py migrate ```
 
