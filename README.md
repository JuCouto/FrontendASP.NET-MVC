# FrontendASP.NET-MVC
Frontend ASP.NET MVC  C#

# Criando um projeto MVC

no terminal digitar -->   dotnet new mvc

ou escolher a opção de projeto ASP MVC no menu inicial do visual studio 2022

***************************************************************************
O ciclo é controller -> View -> Model

criar o Controller e,  seguindo o nome do controller, criar uma pasta com o mesmo nome na view e criar as classes do
tipo cshtml dentro da view, seguindo os nomes das páginas criadas no controller(métodos).

ex:ContatoController  -- criar pasta Contato dentro da pasta View  -- (criei a pasta Index)

*Analisar a necessidade de criar as páginas(classe.cshtml) de acordo com as rotas sugeridas no controller (métodos)

**************************************************************************

# Configurando o Entity framework Core:

- instalar pacote para Banco de dados (instalei sqlite): dotnet add package Microsoft.EntityFrameworkCore.Sqlite

- instalar pacote design: dotnet add package Microsoft.EntityFrameworkCore.Design

*******************************************************************************

criar model - classe da entidade

*********************************************************
## Conexao com Banco de Dados

criar pasta context - classe agendaContext

desenvolvedor.jason criar a conexão - aqui eu digo qual o nome do meu banco de dados

program.cs-conexão banco

instalar a migration (dar nome descritivo para a migration q será criada)

- dot net ef migration add AdicionaTabelaContato

Criando a tabela no banco de dados:

- dotnet ef database update


**************************************************************************
IEnumerable -- é uma lista ex: IEnumerable<nomedoprojeto.Models.nomedapasta>

@{
        ViewData["Title"] = "Listagem de Contatos"; //nome que aparece na aba do navegador
    }
    
- A pasta SHARED q está no view, dentro tem a classe Layout ela  é responsável pelolayout de todas as paginas , inclusive o menu inicial
