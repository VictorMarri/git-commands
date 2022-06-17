# git-commands

### Criando um repositorio

```sh
git init
```
Dessa forma, o git vai criar arquivos necessários para inicializamos, e o diretório atual será reconhecido pelo Git como um projeto e responmderá aos demais comandos digitados no terminal. Esses arquivos ficarão ocultos na pasta .Git

### Verificando status do Branch

```sh
git status
```
Ao digitarmos esse comando, vamos conseguir ver claramente quais arquivos não estão incluidos no versionamento, ou então quais arquivos que foram alterados e que estão pendentes de adição no versionamento. Basicamente, com isso vamos ver as mudanças feitas no arquivo.

### Adicionando os arquivos não incluidos au alterados no branch
```sh
git add . 
ou 
git add <nomedoarquivo.extensao>
```

### Commitando as alterações 
````sh
git commit -m "Mensagem do commit"

ou

git commit <nomeDoAquivo.extensao> -m "Mensagem do commit"
````

### Criar uma branch (Sem acessar)
```sh
git branch "nome da branch"
````

### Criar uma branch (Acessando automaticamente)
````sh
git checkout -b "nome da branch"
ou
git checkout -b <"Nome da branch pra ser criada"> <"Nome da branch de referencia pra criação">
````

### Enviar o codigo para o repositório remoto
````sh
git push
````
Com esse comando, vamos enviar todas as alterações/commits que fizemos dentro do nosso repositório local diretamente para o nosso repositório remoto, que pode ser por exemplo um GitBucket ou um AzureDevOps
