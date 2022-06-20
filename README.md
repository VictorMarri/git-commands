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

### Recebendo mudanças do repositorio remoto
````sh
git pull
````
Muitas vezes a gente pode trabalhar em projetos em que colegas tambem estão desenvolvendo em branches separados. Quando algum colega acaba de desenvolver primeiro que voce e da um push para o repositorio remoto, todas as alterações vão ficar pendentes de merge quando voce subir para o seu repositorio, caso tenham mexido na mesma linha de codigo em branches diferentes. A ação de sincronizar seu branch local com o repositorio remoto é feita através do comando git pull.

### Clonando Repositórios
````sh
git clone <linkRepositorio>
````

### Removendo arquivos do repositório
````sh
git rm <arquivo>
````
### Removendo arquivo git do repositorio
````sh
git rm .git -force
````
