Análise e Inspeção de Repos
===========================

### Exibindo informações do branch e/ou tag

```
git show

//Exbir informações de tags
git show <tag>

```

Esse comando dá diversas informações úteis do branch atual e tambem seus commits, alem de mostrar modificações de arquivos.

### Exibindo diferenças de um branch

```
//Difernça entre branches
git diff

//Diferença entre arquivos
git diff <arquivoX> <arquivoY>

```

Esse comando serve para **exibirmos as diferenças de um branch.**

Quando utilizado, **as diferenças do branch atual com seu branch HEAD remoto serao exibidas no terminal, sejam elas mudanças de adição ou de remoção de itens/codigo.**

### Log resumido do projeto

```
git shortlog

```

Esse comando **nos dá um log resumido do projeto.**

Cada commit vai ser unido por **NOME DO AUTOR**

E assim podemos **saber quais** **commits foram enviados ao projeto e por quem**
