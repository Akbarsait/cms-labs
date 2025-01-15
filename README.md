# CMS Labs
Experiments and explorations with head-less cms and SSG. 

## Contentful Preview
1. Clone the repo https://github.com/contentful/preview-demo
2. Install dependencies 'npm install'
3. Configure application 'npm run setup'
   1. In case if you receive a mesaage like "You are using Node.js 18.8.0. For Next.js, Node.js version >= v18.17.0 is required.", follow the below steps. 
   2. Run "nvm list" to find out available versions of node in the system. 
   3. If the required version or higher version of it is not listed, execute "nvm install --lts"
   4. Run "nvm list" again to check the latest version. 
   5. Run "nvm use 23.6.0" is the latest version installed. 
4. Now run "npm run dev"