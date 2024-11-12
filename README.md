# Projeto Universitário de Conexão com Banco de Dados em PHP

Este projeto foi desenvolvido como parte das atividades acadêmicas em uma universidade federal, visando a compreensão de conceitos de backend, frontend e conexão com banco de dados usando PHP e MySQL. Ele ilustra a criação de uma aplicação básica com funcionalidades de conexão, inserção, alteração, listagem e exclusão de dados.

## Sumário
- [Descrição do Projeto](#descrição-do-projeto)
- [Funcionalidades](#funcionalidades)
- [Estrutura do Código](#estrutura-do-código)
- [Configuração do Ambiente](#configuração-do-ambiente)
- [Como Usar](#como-usar)
- [Contribuições](#contribuições)
- [Licença](#licença)

## Descrição do Projeto
O projeto consiste em um sistema básico de manipulação de dados com quatro principais funcionalidades:
- Conexão com o banco de dados.
- Inserção de dados no banco.
- Alteração de dados existentes.
- Exclusão de dados.

## Funcionalidades
O projeto permite as operações básicas de CRUD (Create, Read, Update, Delete) em uma tabela chamada `tb_pessoas`, que armazena registros com campos `nome` e `email`.

- **Conectar ao Banco de Dados**: A classe `ConexaoMysql` gerencia a conexão com o banco de dados MySQL.
- **Inserção de Dados**: A classe `GravarDados` permite a inserção de novos registros.
- **Manipulação de Dados**: A classe `Manipular` permite alterar e excluir registros.
- **Teste de Conexão**: A classe `Teste_conecta` permite verificar a conexão com o banco de dados.

## Estrutura do Código
O projeto é composto por várias classes PHP:

- **ConexaoMysql**: Estabelece a conexão com o banco de dados MySQL usando parâmetros locais (`localhost`, `root`, sem senha).
- **GravarDados**: Coleta os dados via POST e utiliza a classe `Manipular` para inserir registros na tabela.
- **Manipular**: Classe que estende `ConexaoMysql` para realizar as operações de inserção, alteração e exclusão no banco de dados.
- **Teste_conecta**: Classe para validar a conexão ao banco.
- **ExcluirDados**: Lê um ID via POST e utiliza `Manipular` para excluir o registro correspondente da tabela.

## Configuração do Ambiente
1. **Clone o Repositório**
   ```bash
   git clone https://github.com/seu-usuario/seu-repositorio.git
   cd seu-repositorio
