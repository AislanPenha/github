# Aprendendo um pouco sobre Git/GitHub
## Iniciando e configurando o GIT
```
git init
git config --global user.name "Aislan Penha"
git config --global user.email "aislan.penha@gmail.com"

```
## Configurar o local do repositório
```
git remote add nomeDoRepositorio endereço

```
>Pode adicionar qualquer nome no **nomeDoRepositorio**, este será o nome que associará com o endereço.

## Listar os repositórios remotos:
```
git remote -v

```
## Remover um repositório remoto:
```
git remote remove origin

```
## Alterar a URL de um repositório remoto:
```
git remote set-url origin NOVA_URL

```
## Alterar o apelido de um repositório remoto:
```
git remote rename origin novo-origin

```
## Configurar o branch
### Visualizar todos os branchs
```
git checkout -a
```
### Entrar na branch e criar nova branch
```
git branch -M master
git checkout -b nova
```
### Escolher um branch, que esteja criado
```
git checkout nova
```
## Fazendo o versionamento
```
git add .
git commit -m "Initial"
```
## Fazendo o pull do versionamento
```
git push nomeDoRepositorio nomeDaBranch
```
>O nomeDaBranch tem que ser a que está utilizando no git, pode utitlizar o comando `git checkout` para visualizar.
![Captura de tela de 2024-01-17 16-25-29](https://github.com/AislanPenha/github/assets/130594608/96c7704a-539c-4c36-9927-bb6374b82908)
>
>Nesse caso, estou usando a branch **design**
## Fazendo o merge
```
git merge novoBranch
git push origin master
```
>Nesse caso, estou fazendo merge do master com novoBranch
## Desfazer alteração
```
git log
```
![Captura de tela de 2024-01-17 17-16-18](https://github.com/AislanPenha/github/assets/130594608/9eb798a6-de50-4225-a11d-dee7b0dc6d4e)
>
>Nesse caso, para apagar a última modificação
```
git reset --hard 399ff80
```
ou usar
```
git reset --hard HEAD~1
```
> HEAD~6: Retornará antes da ultimas 6 alterações
## Fazendo um pull
```
git init
git remote add nomeDoRepsoitorio endereco
git pull nomeDoRepsoitorio
```
## Fazendo um clone
```
git clone endereco
```
## Exibe todos os registros
```
git log
```
## Desfaz um commit 
```
git reverse COMMIT_LOG
```
## Apagar um commit local, que não queira fazer o push
```
git reset --hard COMMIT_LOG_ANTERIOR
```
> O número do commit tem que ser alterior ao que deseja apagar
## Alterando o último commit
```
git comit --amend -m "Nova mensagem"
```
### Texto produzido por: [Aislan Penha](https://github.com/AislanPenha)
