# Configurando o Usuário no Git

No Git, ou como podemos dizer "sua máquina do tempo", podemos e devemos responsabilizar quem fez alterações no projeto. Para tanto, precisamos saber quem de fato foi que mexeu nele. Para isso, fazemos a configuração do usuário no Git, onde você precisa informar seu nome e o email que devem ficar marcados como responsáveis pelas alterações.

## Configuração do Usuário

Para configurar seu nome e email globalmente (para todos os repositórios Git no seu computador):

```bash
git config --global user.name "Seu nome aqui"
git config --global user.email "seu_email_aqui@gmail.com"
```

caso tenha a necessidade de mudar o seu nome e email só em algum projeto, e não globalmente, basta navegar até o projeto e rodar o comando sem a flag ***--global***

```bash
git config user.name "Seu nome aqui"
git config user.email "seu_email_aqui@gmail.com"
```

## Verificar Configurações

Caso tenha a necessidade de verificar o nome e email que você configurou você pode usar

```bash
git config --global --list
```

se você estiver dentro de algum repositório e quiser verificar somente nele, pode rodar o comando omitindo a flag ***--global***

## Criando e adicionando uma Chave SSH ao GitHub

Para facilitar a autenticação com o GitHub e melhorar a segurança, é recomendável usar uma chave SSH. Siga os passos abaixo para criar e adicionar uma chave SSH ao GitHub.

### Passo 1: Gerar a Chave SSh
1. Abra o terminal(Git Bash no windows)
2. Digite o comando abaixo, trocando 'seu_email@gmail.com' pelo seu email:
```bash
ssh-keygen -t rsa -b 4096 -C "seu_email@gmai.com"
```
3. Quando você fizer isso vai aparecer algumas opções, pode deixar tudo no default apertando enter ou modificar caso seja preciso.