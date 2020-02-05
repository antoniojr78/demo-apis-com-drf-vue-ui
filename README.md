# Consumindo APIs Django Rest Framework com VueJs, Bootstrap e Axios / Consuming Django Rest Framework APIs with VueJs, Bootstrap and Axios
Demonstração de front-end em VueJs com Bootstrap e Axios consumindo API back-end em Django Rest Framework para buscar Autores: /  
Front-end demonstration in VueJs with Bootstrap and Axios consuming back-end API in Django Rest Framework to search for Authors: 

[API back-end Django Rest Framework](https://github.com/antoniojr78/demo-apis-com-drf)  

1. Clone o repositório / Clone the repository: 
```bash
$ git clone -b develop https://github.com/antoniojr78/demo-apis-com-drf-vue-ui.git 
$ cd demo-apis-com-drf-vue-ui
```  

2. Instalar Pré-requisitos Node, Npm e vue/cli (uma única vez) / Install Prerequisites Node, Npm and vue/cli(one time): 
```bash
(venv) demo-apis-com-drf-vue-ui$ sudo apt install -y nodejs && sudo apt install -y npm && sudo npm install -g @vue/cli
```  

3. Instalar requerimentos do Projeto / Install Project requirements: 
```bash
(venv) demo-apis-com-drf-vue-ui$ cd my_project-ui && npm install
```  

4. Executar o Servidor / Run the Server
```bash
(venv)~/demo-apis-com-drf-vue-ui/my_project-ui$ npm run serve
```  

5. Será servido no navegador a Lista de Authores da API através da URL: /  
   The API List of Authors will be served in the browser through the URL: 

http://localhost:8080/