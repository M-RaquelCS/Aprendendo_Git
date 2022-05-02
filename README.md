# Aprendendo GIT no MouraTech

## Primeiros passos

De início deve-se criar um diretório local na sua máquina com o seguinte comando:

```
mkdir [nome do diretório]
``` 
ou se você já tenha um projeto em mente e tenha o link do repositório do Github você fará o seguinte comando:

```
git clone [link do repositório]
```
---
Seguindo a ideia que criamos um diretório local, precisamos agora iniciar o git no mesmo com o comando:

```
git init
```
Ao iniciar teremos uma resposta de sucesso:
```
Reinitialized existing Git repository in [caminho do seu diretório]
```
Agora vamos criar uma branch para em seguida commitarmos arquivos criados dentro do diretório:

```
git branch -M main
```
- Atenção: o GitHub usa a branch com o nome main e o git com o nome master, então para publicarmos em um repositório precisamos mudar o nome da branch.

Iremos criar nosso primeiro arquivo de "texto", vamos criar um arquivo do tipo Markdown, .md, que é o tipo desse arquivo que estou usando para explicar, é um arquivo de documentação. comando:

```
echo "qualquer texto" > README.md
``` 

Agora vamos fazer a parte principal, iremos commitar, mas antes precisamos adicionar o arquivo ao git do repositorio:

```
git add README.md
```
ou
```
git add .
```
ou 
```
git add *
```
Nosso primeiro commit:

```
git commit -m "primeiro commit"
```
E pronto primeiro commit lançado ao Git, para ver o histórico do seu Git é com um comando bem simples:

```
git log
```
Com esse comando você terá acesso a todos os dados públicos do commit.

Para publicar em um repositório do GitHub primeiro temos que definir o link de repositório no git para ele saber pra onde mandar os arquivos do seu projeto e etc:

```
git remote add origin [link do repositório]
```
Após esse passo mandamos o comando para o Git enviar os arquivos:

```
git push
```
Caso você esteja trabalhando em grupo ou commitou uma mundaça em outra máquina e quer atualizar os arquivos é bem simples também, dentro do diretório do repositório, faça o seguinte comando:

```
git pull
```
----

## Outros Comandos legais de saber:

### Renomeando arquivos
```
git mv [nomde do arquivo atualmente] [nome do arquivo que você quer]
```

### Verificando os Status dos Arquivos
```
git status
```
ou a versão curta
```
git status -s
```
