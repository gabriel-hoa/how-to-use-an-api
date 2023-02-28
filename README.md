# how-to-use-an-api
Let me show how to request and use a API with React. Basic fundaments about use/consume/request a Web AP. 

First of all let's create a react project

Type on your TERMINAL: "npx create-react-app <name_of_project_react>"

Let's assume here that I will create a project with name "api", so:

"npx create-react-app api"

*NPX is used by NPM for create packages without a global installation(i -g)

After created project with sucess
type: "cd api"
type: "code ."  (this will open the project on VisualStudioCode)

Open the terminal on VSCode( CMD + J)
type: "npm start"


Start cleaning the projects REMOVING(DELETE) the following paste:
App.test.js 
setupTests.js
logo.svg
README.md

At App.js remove all the code writing between <header></header>

Now let's install Axios and React-Router-Dom after:

TERMINAL:
type: "npm install axios"
type: "npm i react-router-dom"

Now let's create the paste structure 

At paste SRC let's create 2 more pastes: "pages" and "services"

At "pages" let's create 3 more pastes: 
"assets" where will be the images
"principal" where will be the initial page
"products" where will be the components for acess the API and return the products

At "services" let's create the arquive "api.js" with the following code:

import axios from "axios";
const api = axios.create({
    baseURL: "https://localhost:7090",
)};
export default api;


