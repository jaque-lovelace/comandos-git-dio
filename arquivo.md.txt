# Comandos básicos no Git:

 ## 📍 Manipulando arquivos de texto:

### 📄Para criar um arquivo de texto dentro de repositório já existente:

```
touch nomedoarquivo.md ou nomedoarquivo.txt;
```

### 📄✅Para salvar esse arquivo:
```
esc + :w
```
### ✅➡️Para salvar e sair:**
```
esc + :wq
```
### ➡️Somente sair:

```
esc +:q
```


## 📍Configurações:

### ⚙️Listar configurações:

```
git config --global --list
```

### 🧼limpando as configurações anteriores de nome ou e-mail:

```
git config --global --unset user.email"meuemail@gmail.com"
```

``` 
git config --global --unset user.name"Meu Nome"
```
```
git config --global --unset user.nickname"meu-apelido"
```

 ### ⚙️Configurando nome ou e-mail:
 
```
 git config --global --user.email"meuemail@gmail.com"
```

```
 git config --global --user.name "Meu Nome"
```

```
 git config --global --user.nickname"meu-apelido"
```

### 🎨Configurando as cores de interação:

```
git config --global color.ui.true
```

## 📍Diretórios:

### 📁Criando um diretório/pasta:

```
 mkdir nomedapasta
```

### 📁Acessar o diretório:
```
cd nomedapasta/ 
```
> Aqui é necessário se atentar para o caminho correto da pasta.
> Ex.: se quero acessar a pasta java que está dentro da pasta Documentos e essa por sua vez está dentro pasta Linguagens dependendo de onde é o ponto de partida ficaria algo assim:

```
cd Documentos/Linguagens/java
```

## 📍Estágios do Git:

### 🚦Mostra a situação do meu arquivo:

```
git status 
```

>se estiver como **untracked** significa que está no primeiro estágio

### 🚦Preparar para commitar:

```
git add nomedoarquivo.txt
```

> Se aparecer  **Changes to be committed** (segundo estágio e pronto para ser comitado quando ele **entra para o controle de versão e recebe um *hash* **)

### 🚦Se quiser voltar para unstage, ou seja, para o primeiro estágio untracked:

```
git rm --cached nomedoarquivo.txt
```

### 🚦Para commitar de fato o arquivo ou diretório:
```
git commit -m "Escreva aqui a mensagem inicial do seu commit"
```

💫 e agora ele está comitado e no **stage** (já faz parte do controle de versão)


## 📍Passo a passo simples iniciar projeto:

```
 git init
 ```
 ```
 git add .
 ```
 ```
 git commit -m "Criação do projeto" //quando for a primeira versão
 ```
 ```
 git branch -M main
 ```
 ```
 git remote add origin https://github.com/meu-perfil-github/nome_diretório_arquivo.git 
 ```
 ```
 git push -u origin main
 ```

### 🔧Manutenção do código:

```
git status
```
```
git add .
```
```
git commit -m "nome da versão"
```
```
git push -u origin main
```

