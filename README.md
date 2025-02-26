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

## NextJS Demo 
1. Run the following command. 
   ```zsh
      npx create-next-app --example cms-contentful cms-contentful-app
   ``` 
2. Create Contentful space. Free account is good to start. 
3. Run this command by replacing it with your space ID Content Management Token. 
   ```zsh
      npx cross-env CONTENTFUL_SPACE_ID=YOUR_SPACE_ID CONTENTFUL_MANAGEMENT_TOKEN=XXX npm run setup
   ```
   
4. Create a file .env.local with the following values. 
```zsh
   CONTENTFUL_SPACE_ID=your Space ID
   CONTENTFUL_ACCESS_TOKEN=Content Delivery API token
   CONTENTFUL_PREVIEW_ACCESS_TOKEN=Content Preview API token 
   CONTENTFUL_PREVIEW_SECRET=any URL friendly value of your choice
```
5. Run the following commands
   ```zsh
      npm install

      npm run dev
   ```

## ReactJS Demo 
1. Get the code from repo or clone it to the local. 
2. Run the following command. 
   ``zsh
      npm install
   ``
3. Rename .env.local to .env and update YOUR_SPACE_ID, YOUR_DELIVERY_TOKEN and YOUR_MANAGEMENT_ACCESS_TOKEN with the correct values.
4. Import content model 
   ```zsh
      npm run setup
   ``
5. Run the following command to build local or Prod
   ```zsh
      npm run dev 

      or 

      npm run build
   ```
6. Preview can be accessible at http://localhost:1234 