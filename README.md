# First-REACT

-> Instalar node
    - Penultima aba marcar checkbox

-> Na IDE
    - Verificar se node tá instalado
        - ` node -v `
    - Usar o node pra criar um novo projeto Vite
        - Seguir o passo a passo na documentação
            - Fazer pelo tutorial do ` npm `
        - npm create vite@latest
            - nome o projeto
            - Usar template do react
            - JavaScript
        - executar os comandos informados
            - cd diretorioDoProjeto
            - npm install
            - npm run dev
    - Sempre estar na raiz projeto para trabalhar!

-> Desenvolvimento
    - index.html
        - Página inicial (única página html?)
        - div id=root
            - Dentro dele é onde tudo ocorre
    - src/
        - assets/
        - public/
            - onde está o vite
        - main.jsx
            - vai controlar a raiz do projeto (id root)
            - renderiza a aplicação `<App />`
                - `<App />` foi importado o ./App.jsx
    - App.jsx
        - vai retornar conteúdo da página
        - ele tem um gerenciador de estado de exemplo
        - quando usa <> quer dizer que vai colocar (o retorno) direto dentro do element pai
        - se for usar css, basta importer (import ` archive.css `)
	- Criar um novo componente
		- no ` src/ ` criar uma nova pasta ` components/ ` (respeitar axe para npm conseguir car os diretórios)
			- Criar o ` MeusDados.jsx `
			- páginas podem ser todas index.jsx is por padrão eles procuram index.js em cada pasta de componente
		- function MeusDadosCard() {return (código "html" do javascript)}
		- Após criar o componente, é necessário poder a exporter (export default MeuComponente;)
			- Lá no App.jsx tem que dar o import do componente criado (import MeuComponente from './components/MeuComponente';)
				- Faz oq quiser com ele no App.jsx

# Rotas
oi
- Trazer dependencia para utilizar rotas
       - npm install react-router-dom
  - No main.jsx fazer:
    - import {createBrowserRouter} from 'react-router-dom';
    - const router = createBrowserRouter(
        [
           {}            // Lista de rotas
        ]
      );
    - Substituir o <App/> por <RouterProvider router = {router}>
  
quando usar o a href, pode usar o <Link to='/about'>link</Link> 