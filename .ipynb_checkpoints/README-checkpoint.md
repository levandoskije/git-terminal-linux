# Como usar Git e GitHub no Ubuntu
![Ubuntu/Git Logo](/logo-git-ubuntu.png)  

Nesse repositório irei escrever um resumo dos principais comandos do git  

## Principais comandos
### Iniciando seu primeiro repositório
1. **Download do git**  
[Aqui](https://git-scm.com/download/guis)  
ou  
```
sudo apt-get install git
```
2. **Interface**  
O download da interface recomenda _não é obrigatório_: [GitEye](http://www.collab.net/downloads/giteye)  

3. **Iniciando um repositório**  
- Abra um diretório no seu PC (pasta), com o nome desejado.  
- Abra o terminal neste diretório e de o comando:  
```
git init
```
- Crie o arquivo **README.md**  
```
gedit README.md
```
- Esse arquivo que você está lendo é do tipo Markdown para ver a sintaxe clique [aqui](https://guides.github.com/features/mastering-markdown/)  
- Faça seu primeiro commit  
```
git commit -m "Criando o arquivo Markdown"
```
4. **Crie um repositório no GitHub**  
- Abra sua conta no GitHub  
  - Vá para _repositories_  
  - Abra um novo _New_  

Não é necessário ter o mesmo nome, mas é recomendado  
Após isso o GitHub irá exibir:  
```
git remote add origin <esse link o próprio GitHub fornece>
git push -u origin master
```
### Atualizações no repositório
```
git add .
```
Manda para monitoramento todos os arquivos do diretório, assim como as ações efetuadas
```
git status
```
Mostra o status do diretório
```
git commit -m "mensagem"
```
Adiciona uma mensagem de commit
```
git log
``` 
Mostra o histórico de commits efetuados
```
git push
```
Envia os commits efetuados para o repositório online  
```
git pull
```
Resgata do repositório online os commits efetuados  

### Mais comandos
```
git diff
```
Mostra a diferença entre seu último commit e o atual
```
git diff HEAD~2
```
Mostra a diferença entre seu último commit _HEAD_ até o penúltimo _~2_  
Pode ser digitado qualquer número  
#### Usando Branches
```
git checkout -b NovaBranch
```
Cria uma nova branch chamada _NovaBranch_  
Uma nova branch é um novo ramo de desenvolvimento, que pode ser unido ao principal _Master_ posteriormente  
```
git checkout master
```
Retorna para a branch master  
Se vc fizer o push quando estiver na master, a _NovaBranch_ não será enviada  
```
git branch -d NovaBranch
```
Exclui a branch _NovaBranch_ 
```
git push origin <NovaBranch>
```
Manda para o repositório remoto _GitHub_ a _ NovaBranch_  
```
git merge <branch>
```
Faz merge da sua Branch ativa com a _branch_ indicada  
```
git status
```
Consegue ver qual _Branch_ está ativa  
Provavelmente dará conflitos nos arquivos, sendo assim você terá que arrumar isso  
Após consertar os conflitos, faz uma atualização do repositório novamente  
```
git diff <branch origem> <branch destino>
```
Mostra a diferença entre as Branchs antes de fazer o merge  
É aconselhável escrever _Merged <branch origem> <branch destino>_ na hora de fazer o commit de merge  

### Criando versões _tags_ 

```
git tag v1.0.0 <id do commit desejado>
```
Pode criar tags de versões estáveis do programa

```
git checkout v1.0.0 
```
Entra na versão da tag desejada
```
git -b OutraBranch
```
Cria uma nova branch a partir da _tag_ v1.0.0
```
git checkout master
```
volta para o ramo principal
