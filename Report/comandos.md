## `git init`  
Cria um diretório oculto chamado `.git` dentro da pasta do projeto em desenvolvimento.  
Essa subpasta transforma a pasta atual em um repositório Git, armazenando todas as informações necessárias para o controle de versão.

## `git add .`  
Esse comando serve para adicionar todas as alterações feitas no projeto, como: novos arquivos, modificações em códigos existentes, entre outros, à área de preparação (staging area).

**Obs:** caso queira adicionar um arquivo com nome que contém espaço, você precisa colocá-lo entre aspas duplas `""`.  
Já no comando `git commit -m`, você **sempre** precisa usar aspas duplas para a mensagem.

### Exemplos de uso do comando com e sem aspas abaixo:

`git add novo-arquivo`  
`git add "novo arquivo"`

## `git commit -m`  
Comando que salva as alterações preparadas na staging area, criando um registro (commit) com uma mensagem que explica o que foi feito no projeto.  
Esse commit fica armazenado localmente até que você envie para o GitHub com o comando `git push`.  
Exemplo de uso do comando:  
`git commit -m "adicionando nova função"`

## `git push`  
Como dito acima, esse comando faz parte da etapa final para confirmar as alterações e enviá-las para a plataforma **GitHub**.  
Por padrão, ele envia as alterações para a **branch** ativa (a branch em que você está no momento).  
Se quiser enviar para outra branch, pode usar, por exemplo: `git push origin develop`

## `git pull`  
Esse comando serve para atualizar o seu repositório local com as alterações feitas por outras pessoas no repositório remoto.  
Ou seja, ele "puxa" a versão mais recente do projeto do **GitHub** para o seu computador, mantendo tudo sincronizado.

**Obs:** É importante verificar em qual branch as alterações foram feitas, para garantir que você está baixando a versão correta.  
Por exemplo, em um cenário real, a pessoa pode ter enviado as mudanças para a branch `develop`, e não para a `main`.

## `git status`  
Comando muito importante para analisar as alterações feitas no projeto.  
Com ele, você consegue visualizar quais arquivos foram modificados, adicionados ou removidos, e o que ainda precisa ser commitado.

## `git reset --hard HEAD`  
Comando usado para descartar todas as alterações não commitadas.  
Ele faz o projeto voltar exatamente ao último commit, apagando mudanças feitas nos arquivos e na área de staging.

## `git log`  
Esse comando serve para mostrar o histórico de commit.

## `git diff`  
É um comando útil quando você precisa ver o que foi feito antes de dar `git add`.

## `git clone`
Com esse comando, você clona todo o repositório de um projeto. Ele é interessante porque, ao criar um repositório com um `README.md`, por exemplo, ao dar o clone a sua pasta local já virá com o diretório `.git` e todos os arquivos do projeto prontos para uso.
