# Install REACT 
1) vite download.  
>*npm create vite@latest [project name]*

2) install all dependencies.
>*npm install*

3) run project.
>*npm run dev*    


### More preferred installations before working on a real project:  

* Tailwind CSS - To Improve CSS design. See: [Tailwind CSS](https://tailwindcss.com/docs/installation/using-vite).
    * Install Tailwind CSS.
    >*npm install tailwindcss @tailwindcss/vite*.

    * Configure the Vite plugin in File **vite.config.ts.** add:  
    >*import { defineConfig } from 'vite'.  
      import react from '@vitejs/plugin-react'.  
      import tailwindcss from '@tailwindcss/vite'*
      
        >*export default defineConfig({  
          plugins: [react(), tailwindcss()],  
        })*

    * Import Tailwind CSS to file src/App.css.  
    >*@import "tailwindcss";*  
    
    * Install in VSCode


* install react-router-dom - for client side.  
    >*npm install react-router-dom*

* install axios JS - for client side.  
  for javascript and html project: in your public/index.html file
[<script src=https://cdn.jsdelivr.net/npm/axios@1.6.7/dist/axios.min.js">]

In a react project:
> npm install axios  
  and in a js file or ts file:     
  import axios from 'axios';


In a clean new backend folder  
* create an index.js file
* npm init
* install EXPRESS JS - for server side.
>*npm install express*

* install bcrypt - 
    for password encription - for client side

* install cors (Cross-Origin Resource Sharing).  
    The CORS mechanism supports secure cross-origin requests and data transfers between browsers and servers. 
    
* install mongoose.  
    for MongoDB database connection

* install dotenv.  
    for loading environment variables from a .env file into process.env.


Explain REACT    
-------------
1) App.jsx - All functions start with capital letter.
2) Expression must return one parent element.
3) Each jsx function is a component.
4) Make a components folder for all jsx folder.
5) RFC - React functional component

6) Pass parameters to a component
   a) In App.jsx - using the component
      const nm = user.name; (A js string nm = "Ben".
      
      <SighnUp myName = {nm}></SighnUp>
    
   a) In function SighnUp.jsx - 
   
   >*export default function SighnUp(myProp) {.  
   myProp is allways an object like this.  
   myProp = { myName: "Ben }.    
   so to get the name you have to.  
   cont name = myProp.myName.  
   console.log(myProp)         // = {{myName: "Ben"} }
   const name  = myProp.myName // = {myName: "Ben"}.  
   console.log(name)           // = "Ben".  
   return (...)
   }*
   
### React Hooks
   React hooks are special functions that let you add extra features to your React components.
   1) useState - 
      Is like creating a special variable that React keeps track of.
      When this variable changes, React automatically updates your component.
  
