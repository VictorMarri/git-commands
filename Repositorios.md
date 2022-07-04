Git Repos
=========

### Encontrar Branches

Branchs novos são criados o tempo todo, e o nosso git pode não estar mapeando eles. Podemos pegar por exemplo um caso de alguma alteração que estejamos fazendo, e durante nosso desenvolvimento, um colega cria outro branch pra outra alteração, e por N motivos voce deseja mergear com esse branch do seu colega. Acontece que, ele criou depois de voce ja ter dado um checkout no seu branch, e o seu git acaba não mapeando ele.

```
git fetch

```

Com esse comando **somos atualizados de todos os branches e tags que ainda não são reconhecidas por nos.**


### Atualizar Branch (Dar um pull no branch)

```
git pull

```

Esse comando serve para **recebermos atualizações do repositorio remoto e inserir elas no repositorio local.**

Cada branch pode ser atualizado com esse comando, onde utilizamos para atualizar a master do repo como tambem quando trabalhamos em conjunto e queremos receber atualizações de um dev.


### Enviando alterações (Push nas alterações)

```
git push

```

O Comando **git push** faz o inverso do pull, **enviando as alterações para o repositorio remoto.**

**Usamos esse comando geralmente quando terminamos uma tarefa ou uma serie de commits e queremos enviar tudo para o repositorio remoto.**

**Pode ser usado tambem para enviar atualizações de um branch especifico para outro dev**

Aqui abaixo podemos ver que, quando damos um git status, o git trackeia dois tipos de arquivos: Criados e Modificados:

E o que o comando push prega é que **sejam enviados somente arquivos commitados. Por esse motivo devemos sempre nos atentar que, o arquivo criado não foi trackeado, como podemos ver nessa imagem acima. Por isso é sempre importante verificarmos os arquivos trackeados dando um git status.**

Se não nos atentarmos a isso, o push vai somente nos arquivos trackeados e podemos ter perda de arquivos se não atentarmos.

**Somente damos push em arquivos foram trackeados e commitados.**

### Adicionar, Remover ou trackear um Repositorio novo

Quando a gente cria um **repositorio remoto,** adicionamos ele ao git com **git remote add origin <link>**

```
//Verificando quais as origens para receber e enviar codigo (Trackeando)
git remote -v

//Removendo as origens tanto de fetch (receber) quanto enviar (push) (Removendo)
git rm origin

//Adicionando uma nova origem para o repositorio (Adicionando)
git remote add origin <link>

```

### Submodulos

Submodulas é uma **maneira de possuir dois ou mais projetos dentro de um mesmo repositorio.**

A gente pode adicionar uma dependencia ao nosso projeto atual, porém mantendo suas estruturas separadas.

```
git submodule add <linkRepositorio>

```

Exemplo:

→ Crio um novo repositorio no meu GitHub, e pego o link dele:


→ Adiciono um submodulo dentro do repositorio 1


→ Agora, se repararmos, dentro do nosso projeto agora existe uma pasta chamada Submodulo (Que dei esse nome pra ela. Caso nao desse, ela estaria com o nome padrão do projeto no github)


E quando abrimos essa pasta existe literalmente um projeto inteiro ali, dentro de outro.
