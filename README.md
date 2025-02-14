# DIO | Resumos Git e GitHub

Repositório para armazenar resumos sobre Git e GitHub do curso Versionamento de Código com Git e GiHub da [Digital Innovation One](https://www.dio.me/).

## 📚 Documentação
- [Documentação Git](https://git-scm.com/doc)
- [Documentação Github](https://docs.github.com/)


## 📄 Resumo das Aulas sobre Git

A primeira coisa que você deve fazer ao instalar Git é configurar nome de usuário e e-mail. Isto é importante porque cada commit usa esta informação, e ela é carimbada de forma imutável nos commits que você cria.

```bash
  $ git config --global user.name "Fulano de Tal"
  $ git config --global user.email fulanodetal@exemplo.br
```

Você pode usar o seguinte comando para listar todas as configurações que o Git
```bash
  $ git config --list
```

### 💻 Comandos Git

Alguns comando que achei mais importantes para iniciar no Git. Posteriormente irei acrescentando mais.

- git config --global credential.helper store ou cache

### Comandos
- **git init** : Cria um novo subdiretório chamado .git que contém todos os arquivos necessários de seu repositório.
- **git add <nome-do-arquivo>** : Adiciona o arquivo informado na **staging area**. Isso significa que você está marcando o arquivo especifico para serem incluídos no próximo "commit".
- **git add .** : Usado para adicionar todos os arquivos e mudanças no diretório atual na **staging area**.
- **git status** : Usado para exibir o estado atual do repositório. Mostra informações sobre as mudanças que foram feitas e ainda não foram commitadas.
- **git commit -m "mensagem-descritiva"** : Usado para salvar as mudanças adicionadas a **staging area** em um novo commit. Como se estivesse feito uma captura instantânea do estado atual dos arquivos. **-m** usado para adicionar uma mensagem descritiva, que ajuda a explicar as mudanças que fez.
- **git log** : Exibe o histórico de commits no repositório.
- **git restore <nome-arquivo>** : Usado para reverter mudanças em arquivos no diretório de trabalho e na **staging area**. Para restaurar um arquivo no diretório para a última versão commitada.
- **git restore --staged <arquivo>** : Para remover o arquivo da **staging area**
- **git restore .** : Restaura todas as alterações feitas no diretório.


- **git clone <URL>** : Clona um repositório existente.
- **git diff** : Para ver o que você alterou mas ainda não mandou para o stage.
- **git diff --staged** : Compara as alterações que estão no seu stage com o seu último commit.
- **git branch** : Lista todos os branches no repositório.
- **git branch "nome-da-branch"** : Cria um novo branch.
- **git branch -d <branch>** : Deleta um branch.
- **git branch -m "antigo-nome-do-branch" novo-nome-do-branch"** :  Renomea um branch.
- **git checkout <nome-do-branch>** : Troca para um branch existente.
- **git checkout -b <nome-do-branch>** : Cria um novo branch e troca para o novo branch.
- **git merge <nome-do-branch-origem>** : Usado para combinar as mudanças de dois ou mais branches em um único branch. Utilizado a partir da branch que sofreu as mudanças.
- **git rebase** : Usado para mover ou re-aplicar commits de um branch em cima de outro branch. Ele pega cada commit individual do branch atual e os aplica um por um no topo do branch base. Diferente do **merge*, que cria um novo commit para mesclar as mudanças de dois branches.
Primeiro vá para o branch que você quer rebasear:
```bash
  $ git checkout nome-do-branch
```
Em seguida, rebase-o no branch base:
```bash
  $ git rebase nome-do-branch-base
```

## 🔎 Referências

- [Digital Innovation One](https://www.dio.me/)
