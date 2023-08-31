This is a template for creating an [HTML GitBook style](https://bookdown.org/yihui/bookdown/html.html#gitbook-style) **[bookdown](https://github.com/rstudio/bookdown)** book, [hosted on GitHub Pages](https://bookdown.org/yihui/bookdown/github.html). It is based on the one created with *File, New Project..., New Directory, Book Project using bookdown* in RStudio. It assumes you know how to use git/GitHub and R Markdown, and have some familiarity with the **bookdown** package. If you don't, the package author Yihue Xie's RStudio webinar *[Introduction to Bookdown (R Package)](https://www.youtube.com/watch?v=dVqVscgwSpw)* provides an excellent introduction. In addition, check out [*bookdown: Authoring Books and Technical Documents with R Markdown*](https://bookdown.org/yihui/bookdown), also by Yihui Xie, both for the content and the format--it is itself a **bookdown** book.
If you need help getting git/GitHub to work with RStudio see: [Happy Git and GitHub for the useR](https://happygitwithr.com/) by Jenny Bryan.


## ABSOLUTE ESSENTIALS

*If you have any difficulties or have feedback of any kind, please file an issue or communicate through [Discussions](https://github.com/jtr13/bookdown-template/discussions).*

### Copy this template (GitHub)

- [ ] 1. Click the green "Use this template" button above. DO NOT FORK THE REPO. Choose a descriptive name for your repo based on your content. (Unlike when you fork a repo, you get to choose the name. If you change your mind before you do any work, delete your new repo and start over.)

### Set up Pages (GitHub)

- [ ] 1. On the home page of your repo, click Settings. Click the "Pages" section on the left. In the **Build and Deployment** section, set **Source** to "Deploy from a branch" (Classic Pages experience) and **Branch** to **main** with **/docs** folder. Click Save. Above the **Build and Deployment** section, a box will appear with your book's URL. Copy the URL. (Note that sometimes there is a delay until your book actually appears at that URL. If it doesn't appear after a few minutes, make a change and commit it to trigger a GitHub Pages build.)	

- [ ] 2. Click the gear button near "About" on the home page of the repo and paste your book URL into the **Website** field that appears on the right.

### Copy the repo link (GitHub)

- [ ] 1. Click the green Code button and copy the link under HTTPS. It should have the format: `https://github.com/[USERNAME]/[REPO NAME].git`

### Clone o repositório no RStudio

1. Clone seu novo repositório em *Arquivo > Novo Projeto... > Versão Controle > Git* no programa [RStudio](https://posit.co/download/rstudio-desktop/). Você precisará colar o link do passo anterior na caixa de diálogo para o URL do Repositório.

### Edite alguns arquivos chave usando o RStudio

1. No arquivo `index.Rmd`, mude INSIRA SEU TITULO AQUI para o título do seu livro.

2. No arquivo `index.Rmd`, mude INSIRA SEU NOME AQUI para o seu nome.

3. No arquivo `_bookdown.yml`, mude SEU NOME DE USUARIO GITHUB para o seu nome do usuário no Github, nos dois lugares em que aparece.

4. No arquivo `_bookdown.yml`, mude NOME DO SEU REPOSITORIO para o nome do seu repositorio do livro no Github, nos dois lugares em que aparece.

(Note que os passos 3 e 4 fornecem links para os arquivos `.Rmd` do seu projeto para edição e visualização. Se você mover seus arquivos `.Rmd``você terá que atualizar o caminho para esses arquivos. Uma vez o livro estando renderizado, teste se os butões para editar (caneta) e visualizar (olho)estão funcionando.)

5. No arquivo `_output.yml`, mude TITULO CURTO AQUI para uma versão encurtadado seu título. 

(Deixe as informações da linha seguinte a "after:" para indicar que seu livro foi publicado com bookdown na forma que está.)

### Como renderizar o livro

1. Instale **bookdown** com o comando `install.packages("bookdown")`. Se você já o tem, atualize-o para a [última versão](https://CRAN.R-project.org/package=bookdown).

2. Renderize (*render*) localmente com o comando `bookdown::render_book("index.Rmd")`.

3. Use o comando `browseURL("docs/index.html")` para ver o livro localmente (ou simplesmente abra o arquivo `index.html` em um navegador).

4. Se a versão renderizada lhe agrada, comprometa (*commit*) e envie (*push*) todos os arquivos modificados para o GitHub. 

5. Vá ao GitHub, usando o comando `usethis::browse_github()`.

Você precisará repetir os passos 2 e 4 todas as vezes que quiser atualizar o livro online.


### Edite o arquivo `README.md` usando GitHub ou RStudio

Depois de concluir essas etapas, exclua o conteúdo deste arquivo e adicione uma breve descrição do seu projeto, com um link para o URL do livro. Agradeceríamos se você adicionasse o seguinte ao final:

*Este repositório foi gerado inicialmente a partir de um modelo de bookdown disponível aqui: https://github.com/depaulats/modelo-bookdown/*


### Informações adicionais

Este repositório foi gerado inicialmente a partir de um modelo de bookdown disponível [aqui](https://github.com/jtr13/bookdown-template).

Por favor consulte o vídeo demostrativo de [como criar um livro **bookdown**](http://bit.ly/fiveminutebookdown) e o [guia oficial do **bookdown**](https://bookdown.org/yihui/bookdown). 
