Aqui você vai encontrar todos os arquivos base de modelo para criar um livro no estilo [HTML GitBook](https://bookdown.org/yihui/bookdown/html.html#gitbook-style)  **[bookdown](https://github.com/rstudio/bookdown)**, [hospedado nas páginas do GitHub](https://bookdown.org/yihui/bookdown/github.html). Este modelo foi adaptado para o português, tendo como base um projeto criado no RStudio pelo caminho *Arquivo > Novo Projeto... > Novo Diretório > Projeto de Livro usando bookdown*.
Este tutorial passo-a-passo assume que você saiba usar git/GitHub e R Markdown, e tem alguma familiaridade com o pacote **bookdown**. Caso contrário, Yihue Xie, o autor do pacote bookdown, possui um webinário de {Introdução ao Bookdown](https://www.youtube.com/watch?v=dVqVscgwSpw) excelente (em inglês). Veja também outro livro do autor, [*bookdown: Authoring Books and Technical Documents with R Markdown*](https://bookdown.org/yihui/bookdown).
Se precisar de ajuda para colocar o git/GitHub para funcionar com o RStudio, veja o tutorial de Jenny Bryan [Happy Git and GitHub for the useR](https://happygitwithr.com/). 


## Importante

*Se você tiver qualquer dificuldade em usar este repositório, por favor [registre um problema](https://github.com/depaulats/modelo-bookdown/issues).*


### Copie este modelo no GitHub

1. Clique no butão verde acima "Use este modelo" (*Use this template*). NÃO USE A OPÇÃO FORK. Dê um nome descritivo para o seu repositório de acordo com o conteúdo que deseja produzir. (Ao contrário do Fork, aqui você pode escolher o nome. Se mudar de idéia logo no início, apague seu repositório, e comece novamente).

### Configure as páginas do GitHub

1. Na página de início (*home*) do seu repositório, clique em configurações (*Settings*). Clique na seção "Páginas" (*Pages*) à esquerda. Na seção "Construção e Implantação" (*Build and Deployment*), defina a "Fonte" (*Source*) para "Implantar a partir de uma ramificação" (*Deploy from a branch*) e a "Ramificação" (*Branch*) para "principal" (*main*) com pasta "/docs". Clique em "Salvar" (*Save*). Acima da seção "Construção e Implantação" (*Build and Deployment*), um caixa de diálogo irá aparecer com a URL do seu livro. Copie a URL. (Note que algumas vezes há um atraso até que o livro aparece na URL. Se ele não aparecer após alguns minutos, mude e submeta (*commit*) algum arquivo para acionar a contrução das Páginas do GitHub.)GitHub Pages build.)	

2. Clique no butão de engrenagem perto de "Sobre" (*About*) na página inicial do repositório e cole a URL do seu livro no campo "Website" que aparece à direita.

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
