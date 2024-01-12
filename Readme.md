# Git Course

Este é um repositório teste para ensinar como git funciona.


Saiba mais em [willianjusten.com.br](https://willianjusten.com.br)

# Comandos e dicas

git config --global user.name "nome de usuario"
git config --global user.email "email do usuario"
 
** configurando usuário e email **


git config --global --unset user.name 
git config --global --unset user.email

** removendo usuário e email **

O git guarda suas infomrações de três coisas

sistema
usuario -> global
projeto

# Vendo as configurações

``git config user.name`` mostra o usuario
``git config user.name`` mostra o email
``git config core.editor`` mostra editor padrão
``git config --list`` mostra todas as informações


mkdir -> criando pastas

git init -> iniciando repositório local

vi readme.md -> criando arquivo readme

i -> entrar no modo insert

esc :wq -> salvar e sair

_Ciclo de vida dos status dos arquivos

untracked (arquivo acabou de ser adicionado no repositorio mas o git ainda não viu ele)

| git add nome-do-arquivo -> Torna o arquivo visivel no git
v  

unmodified (adicionou o arquivo no git, mas não foi modificado)


modified (se você modifica o arquivo)


staged (area onde você cria a versão)

-> git commit -m "mensagem"


Assim que você fizer o commit todos os arquivos voltam a ser unmodified)

comando ``git status`` -> Reportar como está o seu repositório no momento


COMMIT -> momento que você fala pro git pegue esses arquivos e crie uma imagem dele (uma versão)
você só consegue commitar depois que adicionou as modificações


# Vendo as versões com log

comando ``git log`` para conseguir ver as versões

comando ``git log --decorate`` para mais informações

comando ``git log --author="nome-do-autor"`` filtrar por autor

comando ``git shortlog`` mostra as versões de forma resumida

comando ``git shortlog -sn`` mostra os contribuintes e a quantidade de contribuições

comando ``git log --graph`` mostra os logs de forma gráfica

comando ``git diff`` mostra as alterações antes de realizar um commit

comando ``git diff --name-only`` mostra apenas os nomes dos arquivos modificados


# Selecionando uma versão

Cada versão possui uma **hash**, que é um identificador 

comando ``git show hash-numero`` consigo ver o que foi a adicionado nela


# Commitando um arquivo que já existiu sem utilizar o add

``git commit -am "mensagem"``

