# Como integrar o Github a um projeto na sua Máquina

### Com o git já instalado

Abra o VSCode no seu projeto, nele abra o terminal e 
execute seu ambiente virtual, logo depois o comando:
```bash
git init
``` 

Em seguida, faça:
```bash
git add .
``` 
Esse comando adiciona todos os arquivos do projeto na área de stagging.

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

<img src="">

mas o que você tem que fazer é bem simples, apenas copie o link que aparecer para você
