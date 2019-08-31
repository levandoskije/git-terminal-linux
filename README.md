# Como usar Git e GitHub no Ubuntu
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
git diff
```
Mostra a diferença entre seu último commit e o atual
```
git diff HEAD~2
```
Mostra a diferença entre seu último commit _HEAD_ até o penúltimo _~2_  
Pode ser digitado qualquer número
