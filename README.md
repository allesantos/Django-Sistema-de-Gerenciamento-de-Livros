# Alleart - Plataforma de Gerenciamento de Livros
 
Este é um projeto de uma plataforma de gerenciamento de livros desenvolvida com Django. 

## Índice
- [Descrição](#Descrição)
- [Recursos](#Recursos)
- [Tecnologias Utilizadas](#Tecnologias)
- [Pré-requisitos](#Pré-requisitos)
- [Instalação](#Instalação)
- [Uso](#Uso)
- [Contribuição](#Contribuição)
- [Licença](#Licença)

## Descrição
**Alleart** é uma plataforma que permite que os usuários se cadastrem, façam login e publiquem informações sobre os livros que possuem. Além disso, os usuários podem emprestar seus livros fisicamente para outros usuários cadastrados ou visitantes, registrar devoluções e avaliar o estado dos livros devolvidos.

**Status do projeto:** Fase Beta — funcionalidades adicionais e melhorias estão planejadas para versões futuras.

## Recursos
- Cadastro e login de usuários.
- Publicação de informações sobre livros.
- Empréstimo de livros para outros usuários ou visitantes.
- Registro de devoluções com avaliação do estado do livro.
- Interface amigável e responsiva.

## Tecnologias Utilizadas
- __Backend:__ Django 4.x
- __Banco de Dados:__ SQLite (padrão)
- __Frontend:__ HTML, CSS, Bootstrap

## Pré-requisitos
Antes de iniciar, certifique-se de ter os seguintes itens instalados:
- Python 3.8 ou superior
- pip (gerenciador de pacotes do Python)
- Virtualenv (recomendado para isolamento do ambiente)
- Git

## Instalação
1. Clone o repositório para sua máquina local:

    ```
    git clone https://github.com/seu-usuario/nome-do-repositorio.git
    cd nome-do-repositorio
    ```

2. Crie e ative um ambiente virtual:

    ```
    python -m venv venv
    source venv/bin/activate  # No Windows: venv\Scripts\activate
    ```

3. Instale as dependências do projeto:

    ```
    pip install -r requirements.txt
    ```

4. Execute as migrações do banco de dados:

    ```
    python manage.py migrate
    ```

5. Inicie o servidor de desenvolvimento:

    ```
    python manage.py runserver
    ```

6. Acesse o sistema em http://127.0.0.1:8000/ no seu navegador.

## Uso

1. Para utilizar o sistema é necessário realizar um cadastro, registrando apenas usuário, email e senha.
Na imagem abaixo, temos alguns exemplos de livros publicados por um usuário.

<img src = "https://github.com/allesantos/allesantos/blob/main/imagens/Biblioteca-Django/01.png">



Para utilizar o sistema é necessário realizar um cadastro, registrando apenas nome, email e senha.

<img src = "https://github.com/allesantos/allesantos/blob/main/imagens/Biblioteca-Django/07.png">



Após o cadastro, é preciso fazer login para ter acesso a sua própria sessão de usuário.

<img src = "https://github.com/allesantos/allesantos/blob/main/imagens/Biblioteca-Django/08.png">


No canto direito da página, após realizar o login, temos um botão de Menu, onde é possível desde realizar cadastro, emprestimo, devolução como também visualizar os livros que alguém emprestou para este usuário e ver o total de livros já publicados.

<img src = "https://github.com/allesantos/allesantos/blob/main/imagens/Biblioteca-Django/02.png">


Clicando em Opções do Menu, temos "Categoria", "Livro", "Empréstimo" e "Devolução". Realize primeiro o cadastro das categorias dos livros que deseja publicar, por exemplo, "Ação", "Romance", "Terror" etc. Quando for cadastrar um livro, você também pode enviar uma imagem que servirá como capa do livro.

<img src = "https://github.com/allesantos/allesantos/blob/main/imagens/Biblioteca-Django/03.png">


Em "Emprestimo" você poderá emprestar seus livros para usuários "Visitante", ou seja que não possui ainda um cadastro no sistema como também para usuários que já possuem um cadastro, basta apenas alternar entre os dois botões.

<img src = "https://github.com/allesantos/allesantos/blob/main/imagens/Biblioteca-Django/04.png">


Quando for acessar a página que possui mais informações sobre um dos livros publicados, nela é possível ainda alterar ou excluir o livro.

<img src = "https://github.com/allesantos/allesantos/blob/main/imagens/Biblioteca-Django/05.png">


Quando for registrar a devolução de um livro que havia antes emprestado para um usuário, é possível avaliar o estado de como foi devolvido o livro. A avaliação será classificada em forma de estrelas.

<img src = "https://github.com/allesantos/allesantos/blob/main/imagens/Biblioteca-Django/05b.png">


Note que não será possível avaliar a devolução de um livro caso o usuário ainda não tenha devolvido para você, sendo assim, o botão "Avaliar" será visualizado, porém indisponível para avaliação.

<img src = "https://github.com/allesantos/allesantos/blob/main/imagens/Biblioteca-Django/05c.png">


