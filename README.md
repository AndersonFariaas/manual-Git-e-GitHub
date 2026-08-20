# 🚀 Manual Rápido: Git e GitHub

## 1. O que são Git e GitHub?

**Git** é uma ferramenta usada para **controlar versões dos seus projetos**. Ele registra as alterações feitas no código e permite voltar a versões anteriores.

**GitHub** é uma plataforma online onde podemos **armazenar, compartilhar e colaborar em projetos que utilizam Git**.

### Em resumo:

```text
Git = controla as versões do código
GitHub = armazena o projeto online
```

---

# 2. Criando uma conta no GitHub

Acesse:

**https://github.com/**

1. Clique em **Sign up**.
2. Informe seu **e-mail**.
3. Crie uma **senha**.
4. Escolha seu **nome de usuário**.
5. Confirme seu e-mail.
6. Conclua as etapas solicitadas.

✅ Sua conta GitHub está pronta!

---

# 3. Baixando e instalando o Git

Acesse:

**https://git-scm.com/downloads**

1. Escolha **Windows**.
2. Baixe o instalador.
3. Execute o arquivo baixado.
4. Durante a instalação, mantenha as opções padrão.
5. Clique em **Install**.
6. Ao terminar, clique em **Finish**.

### Verificando a instalação

Abra o **Git Bash** ou o terminal do VS Code e digite:

```bash
git --version
```

Se aparecer algo como:

```text
git version 2.x.x
```

✅ O Git foi instalado corretamente.

---

# 4. Configurando o Git

No terminal, informe seu nome:

```bash
git config --global user.name "Seu Nome"
```

Depois, informe o e-mail usado no GitHub:

```bash
git config --global user.email "seu@email.com"
```

Pronto! O Git está configurado.

---

# 5. Criando seu primeiro projeto

Crie uma pasta para o projeto.

Exemplo:

```text
meu-primeiro-projeto
```

Dentro dela, crie um arquivo:

```text
index.html
```

Exemplo:

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>Meu primeiro projeto</title>
</head>

<body>

    <h1>Meu primeiro projeto com Git!</h1>

</body>
</html>
```

---

# 6. Criando o repositório Git local

Abra o terminal dentro da pasta do projeto.

Execute:

```bash
git init
```

Agora o Git começou a controlar seu projeto.

Confira:

```bash
git status
```

---

# 7. Criando o repositório no GitHub

Acesse:

**https://github.com/**

1. Clique em **+**.
2. Clique em **New repository**.
3. Digite um nome.

Exemplo:

```text
meu-primeiro-projeto
```

4. Escolha **Public** ou **Private**.
5. Clique em **Create repository**.

> Para este primeiro exercício, deixe o repositório vazio. Não marque README, `.gitignore` ou License.

---

# 8. Conectando o projeto ao GitHub

O GitHub fornecerá uma URL semelhante a:

```text
https://github.com/seuusuario/meu-primeiro-projeto.git
```

No terminal do seu projeto:

```bash
git remote add origin https://github.com/seuusuario/meu-primeiro-projeto.git
```

Confira:

```bash
git remote -v
```

---

# 9. Fazendo o primeiro commit

Primeiro, adicione os arquivos:

```bash
git add .
```

Depois crie o commit:

```bash
git commit -m "Primeiro commit"
```

O **commit** é um registro da versão atual do projeto.

---

# 10. Enviando o projeto para o GitHub

Garanta que a branch seja `main`:

```bash
git branch -M main
```

Agora envie o projeto:

```bash
git push -u origin main
```

Pronto! 🎉

Seu projeto agora está no GitHub.

---

# 11. Fazendo uma alteração

Abra o `index.html` e altere, por exemplo:

```html
<h1>Meu primeiro projeto com Git!</h1>
```

para:

```html
<h1>Meu primeiro projeto com Git e GitHub!</h1>
```

Salve o arquivo.

Agora execute:

```bash
git status
```

O Git mostrará que o arquivo foi alterado.

---

# 12. Registrando e enviando a alteração

Execute:

```bash
git add .
```

Depois:

```bash
git commit -m "Atualiza título da página"
```

E envie para o GitHub:

```bash
git push
```

Pronto!

A alteração agora também está no GitHub.

---

# 13. Fazendo um Git Clone

Imagine que você está em outro computador e quer baixar o projeto que está no GitHub.

No GitHub:

1. Abra o repositório.
2. Clique em **Code**.
3. Selecione **HTTPS**.
4. Copie a URL.

Exemplo:

```text
https://github.com/seuusuario/meu-primeiro-projeto.git
```

No terminal, vá até a pasta onde deseja colocar o projeto e execute:

```bash
git clone https://github.com/seuusuario/meu-primeiro-projeto.git
```

O Git criará uma cópia do projeto no computador.

Entre na pasta:

```bash
cd meu-primeiro-projeto
```

Confira:

```bash
git status
```

---

# 🧠 Comandos essenciais

| Comando | Função |
|---|---|
| `git init` | Inicia o Git no projeto |
| `git status` | Mostra o estado do projeto |
| `git add .` | Prepara as alterações |
| `git commit -m "mensagem"` | Registra uma versão |
| `git push` | Envia para o GitHub |
| `git pull` | Baixa atualizações do GitHub |
| `git clone URL` | Clona um projeto |
| `git remote -v` | Mostra o repositório remoto |

---

# ⭐ Fluxo básico para memorizar

### Primeiro projeto:

```text
CRIAR PROJETO
      ↓
git init
      ↓
git add .
      ↓
git commit
      ↓
git remote add origin URL
      ↓
git push
```

### Quando fizer alterações:

```text
ALTERAR CÓDIGO
      ↓
git add .
      ↓
git commit -m "Alteração"
      ↓
git push
```

### Para baixar um projeto existente:

```text
GITHUB
   ↓
git clone URL
   ↓
COMPUTADOR
```

## 🎯 Regra simples

```text
ADD    → preparar
COMMIT → registrar
PUSH   → enviar
PULL   → baixar atualizações
CLONE  → copiar projeto
```

**Com esses comandos você já consegue criar, versionar, publicar, atualizar e clonar projetos usando Git e GitHub.**
