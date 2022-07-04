Git Branches
============

Branches são ramificações do projeto, codigos fontes do projeto seprados em ambientes unicos. É a forma que o git tem que **separar as versões dos projetos.**

Quando um projeto é criado, ele inicia na **branch master.** Geralmente cada nova feature de um projeto fica em um branch separado, e, após a finalizaçãodas alterações **os branches são unidos para ter o codigo fonte final.**

### Visualizar os branches

```
git branch

```

Com esse comando podemos visualizar todos os branches disponiveis nesse projeto

### Criar branch

```
git branch <nomebranch>

```


Sempre que formos criar um branch (na gigante maioria das vezes) vamos partir da master.

### Deletar branches

```
git branch -d <nomeBranch>

ou

git branch --delete <nomeBranch>

```

### Mudar de branch

**Quando alteramos um branch podemos levar alterações que não foram commitadas! Cuidado!**

```
git checkout <nomeBranch> //Aqui mudamos pra um branch já existente

ou

git checkout -b <nomeBranch> //Aqui criamos um branch e mudamos pra ele

```

Esse comando tambem pode ser utilizado para dispensarmos mudanças de um arquivo.


Essas mudanças feitas no arquivo, estarao somente dentro do branch

### Unir branches (MERGE)

Um dos comandos git **mais utilizados.** É Por meio desse comando que recebemos atualizações de outros devs/branches

```
git merge <nomeBranch>

```

### Jogar o codigo 'no lixo' (stash)

```
git stash

```

Esse comando faz com que salvemos as modificações atuais pra prosseguir com uma outra abordagem de solução **e não perder o código. Após o comando stash, o branch será resetado para sua versão de acordo com o repositorio puxado.**

### Verificar codigos que foram 'jogados no lixo' (stash)

```
git stash list

```

### Recuperando o código jogado no lixo (stash)

```
git stash <nomeStash>

ou

git stash apply {0,1,2,...} //Isso funciona depois de darmos um git stash list, e ai vemos a ordem que os stashs estão inseridos.

```

Dessa maneira podemos recuperar a stash feita anteriormente, e continuar de onde paramos com os arquivos adicionados à stash.

### Removendo o codigo que foi jogado no lixo (stash)

```
git stash clear

ou

git stash drop <nomeStash>

```

Quando fizermos isso, vamos perder todo o registro de Stashs anteriores que voce fez. Portanto, esse comando **não tem volta uma vez que foi solicitado.**

### Criando Tags

```
git tag -a <nomeTag> -m "mensagem para descrever a tag"

```

A Tag é diferente do Stash, pq **serve como um checkpoint de um branch.** É utilizada para **demarcar estágios do desenvolvimento de algum recurso.**

### Verificando as tags que foram criadas

```
git show //Vendo todas as tags

ou

git show <nomeTag> //Vendo uma tag especifica

```

Alem de podermos ver as tags, **podemos trocar de tags, compreendendo estágios diferentes do desenvolvimento do projeto que você aplicou as tags:**

```
git checkout <nomeTag>

```

Dessa maneira, **podemos retroceder ou avançar e checkpoints de um branch**
