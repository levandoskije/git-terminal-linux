# Como usar Git e GitHub no Ubuntu
Nesse repositório irei escrever os principais comandos do git  

## Principais comandos
### Iniciando seu primeiro repositório
1. **Download do git**
[Aqui](https://git-scm.com/download/guis)  
ou  
```
sudo apt-get install git
```
2. **Interface**
O download da interface recomenda __não é obrigatório__: [GitEye](http://www.collab.net/downloads/giteye)  

3. **Iniciando um repositório**
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
4. **Crie um repositório no GitHub**
* Abra sua conta no GitHub  
* Vá para __repositories__  
* Abra um novo __New__  

Não é necessário ter o mesmo nome, mas é recomendado  
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

