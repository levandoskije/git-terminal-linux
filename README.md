# Como usar Git e GitHub
Nesse repositório irei escrever os principais comandos do git  

## Principais comandos
### Download do git
```
sudo apt-get install git
```
#### Interface
O downoload das interfaces pode ser feito [aqui](https://git-scm.com/download/guis)  
[GitEye](http://www.collab.net/downloads/giteye)  

### Iniciando um repositório
Abra um diretório no seu PC (pasta), com o nome desejado  
Abra o terminal neste diretório e de o comando:  
```
git init
```
Crie o arquivo **README.md**  
```
gedit README.md
```
Esse é um arquivo do tipo Markdown para ver a sintaxe clique [aqui](https://guides.github.com/features/mastering-markdown/)  
Faça seu primeiro commit
```
git commit -m "Criando o arquivo Markdown"
```
#### Crie um repositório no GitHub
Não é necessário ter o mesmo nome, mas é recomendado  
```
git remote add origin <esse link o próprio GitHub fornece>
git push -u origin master
```
