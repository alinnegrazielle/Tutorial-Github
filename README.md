# Como integrar o Github a um projeto na sua Máquina

### Com o git já instalado

Abra o VSCode no seu projeto, nele abra o terminal e 
execute seu ambiente virtual, logo depois o comando:
```bash
git init
``` 
Esse comando cria um repositório .git dentro do seu projeto.

Em seguida precisamos adicionar todos os arquivos já existente do seu projeto para a área de staging do github,
essa área é um local de armazenamento intermediário, situada entre sua máquina e o github. Para isso, digite:
```bash
git add .
``` 

Agora vamos nomear essa versão do projeto que você pretende subir:
```bash
git commit -m "projeto criado"
``` 

Em seguida precisamos alterar o nome da branch principal de `master` para `main` com:
```bash
git branch -M "main"
```

### Iniciando o projeto no Github

Abra o navegar no site do Github e crie um novo repositório, adicionando um nome para o projeto
e uma descrição, feito isso você já pode clicar em criar o repositório.
OBS.: **não precisa adicionar um README**, por isso não marque a caixinha do readme.md

Logo em seguida você vai ser redirecionado para uma página semelhante a essa:

<img src="https://github.com/alinnegrazielle/Tutorial-Github/blob/main/linkremote.png">

Nessa página, apenas copie o link que aparecer para você e volte para o VSCode.


### Integrando o repositório local com o repositório remoto

Para passar o commit da sua máquina para um repositório na plataforma do Github, usamos o comando:
```bash
git remote add origin <cole aqui o link do repositório que vocẽ copiou da página no github>
```
Agora o repositório da sua máquina, já foi conectado com o respositório do Github, porém o commit que damos na máquina não sobe os arquivos automaticamente.
Precismos então retirá-los da área de staging e `empurrar` para a plataforma do github. Utilize o seguinte comando:
```bash
git push -u origin main
``` 

Voltando para o site do github, recarregue a página e vocẽ verá seus arquivos na plataforma!

### Continuando o projeto na sua máquina

Sempre que você fizer alterações no seu projeto e desejar subí-las para o Github, vá ao terminal do VSCode e digite os seguintes comandos:

```bash
# Adicione os novos arquivos na área de staging, com o comando:
git add .

# Em seguida você precisa nomear essa nova versão do seu projeto:
git commit -m "Novas alterações"

# Agora você já pode subir suas mudanças:
git push origin main (sem o -u)

``` 

