# :computer: Tela inscrição da HashTag Treinamentos 
---
:link: Link da página:
Netlify - https://inscricaotelahashtag.netlify.app/inscricao

## Explicando o projeto

Neste Projeto efetuei o treinamento dos meus conhecimentos em Desenvolvimento FrontEnd, replicando a página de incrição de um evento online da hashTag Treinamentos. A Página detalha os itens que serão abordados, os conhecimentos que serão transmitidos e como esse intensivão poderá ajudar o aluno a destacar no mercado e despertar o intersse de possíveis recrutadores. O projeto foi otimizado e tem responsividade para desktop, tablets e mobile.
---
## :clipboard: Tecnologias utilizadas
- Html
- Sass
- Css
- JavaScript
---
## :link: Dependências necessárias
Caso não tenha o node e o sass instalados, abra o navegador, faça os downloads e siga as etapas de instalação.

Verifique se o Node.js e o npm foram instalados:  
cmd  
digite: node -v  
digite npm -v  
se estiverr instalado corretamente ele vai retornar a versão  
feche o cmd e abra o vscode  
abra o terminal  
digite: npm install --save-dev-sass  
Para terminar de baixar as dependências que podem estar faltando digite:  
npm install  


---
## :ballot_box_with_check: Como rodar a aplicação no vscode

Abra o projeto  
Abra um novo terminal (ctrl + shift + ')  
Digite: npm init  
Configure o projeto seguindo no terminal, se não quiser alterar nada apenas aperte enter até ele terminar de criar o package
ao final um package.json será criado  
crie uma pasta css fora da pasta sass  
crie um arquivo "main.scss" na pasta sass  
crie um arquivo index.html fora das pastas  
configure o html  
link o "css/style.css" no index.html, mesmo que o arquivo style.css ainda não estaja criado  
no package.jason substitua o scripts por:  
"scripts": {  
    "watch:sass": "sass sass/main.scss css/style.css -w",
    "compile:sass": "sass sass/main.scss css/style.comp.css",  
    "prefix:css": "postcss --use autoprefixer -b 'last 10 versions' css/style.comp.css -o css/style.prefix.css",  
    "compress:css": "sass css/style.prefix.css css/style.css --style compressed",  
    "build:css": "npm-run-all compile:sass prefix:css compress:css"  
  }  
abra o terminal e rode o comando:   
npm install postcss postcss-cli autoprefixer --save-dev  
npm run build:css  


## :camera: Imagens do Projeto
<img width="1902" height="918" alt="cap1-hashtag" src="https://github.com/user-attachments/assets/e8920845-495c-4550-b529-36221c96ef82" />
<img width="1895" height="874" alt="cap2-hashtag" src="https://github.com/user-attachments/assets/610e9607-cc0a-4b38-b1ef-5f89e5a60ec5" />
<img width="438" height="795" alt="cap3-hashtag" src="https://github.com/user-attachments/assets/15b608e1-44cf-4344-8a61-3b840a419397" />
<img width="442" height="798" alt="cap4-hashtag" src="https://github.com/user-attachments/assets/2f39f6cd-5845-404e-9fdc-d36b222076b3" />
<img width="1899" height="905" alt="cap5-hashtag" src="https://github.com/user-attachments/assets/7d4a16c1-c800-4fd6-b165-e2756e46ba12" />


## :x: Problemas enfrentados
1- Após instalar o node o npm não funcionava
Solucionei o problema abrindo o Prompt de Comando ou o PowerShell como administrador e, em seguida, usar os comandos npm normalmente

2- O Sass apresentava erros
Neste caso foi por erro meu mesmo, que fiz etapas fora de ordem, então neste caso para que o sass funcione corretamente, siga os passos para que as pastas criadas em css estejam corretas.
