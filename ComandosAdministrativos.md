Comandos Administrativos de Git
===============================

### Limpar aquivos não trackeados

```
git clean

```

Esse comando vai **verificar e limpar arquivos não trackeados pelo Git. Esse comando exige certo cuidado pois se voce nao trackear um arquivo importante e digitar esse comando, voce perdeu ele pra sempre.**

→ Vamos supor que aconteceu um erro na nossa aplicação, e, para registros dos logs do mesmo, foram criados varios arquivos que voce nao deseja na raiz do projeto:

E, se a gente der um **git status** aparecem esses arquivos não trackeados:


Esses arquivos não sao interessantes para nos, e, num caso de quem não conhece esse comando, **a pessoa teria que excluir na raiz do projeto esse arquivo. Porem ela só precisar dar esse comando para limpar:**


### Git Garbage Collector

```
git gc

```

Esse comando identifica arquivos **que não são mais necessários e os exclui.**

Esse comando ajuda na **performance** da sua maquina.

### Verificando integridade de arquivos

```
 git fsck

```

Esse comando verifica a integridade de arquivos e sua conectividade, verificando **corrupções em arquivos, e checando se esta tudo certo com nossos arquivos**

### Transformando o repositorio para arquivo

```
git archive --format zip --output master_files.zip master

```

Esse comando transforma nosso repositorio num arquivo compactado.


Pegou todo o meu codigo e fez um zip dele:
