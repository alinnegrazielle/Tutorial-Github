# Como integrar o Github a um projeto na sua Máquina

### Com o git já instalado

Abra o VSCode no seu projeto, nele abra o terminal e 
execute seu ambiente virtual, logo depois o comando:
```bash
git init
``` 
Esse comando cria um repositório .git dentro do seu projeto.

### Iniciando o projeto no Github

Abra o navegar no site do Github e crie um novo repositório, adicionando um nome para o projeto
e uma descrição, feito isso você já pode clicar em criar o repositório.
OBS.: **não precisa adicionar um README**, por isso não marque a caixinha do readme.md

Logo em seguida você vai ser redirecionado para uma página semelhante a essa:

<img src="https://github.com/alinnegrazielle/Tutorial-Github/blob/main/linkremote.png">

Nessa página, apenas copie o link que aparecer para você e volte para o VSCode.

### Integrando o repositório local com o repositório remoto

Para passar as mudanças feitas na sua máquina para o repositório anteriormente criado na plataforma do Github, usamos o comando:
```bash
git remote add origin <cole aqui o link do repositório que vocẽ copiou da página no github>
```

Em seguida precisamos nos certificar de que estamos na branch correta e/ou criá-la, caso ainda não exista.
```bash
git checkout -b main
```

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

