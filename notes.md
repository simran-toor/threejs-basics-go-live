# 14 GO LIVE 
## SOLUTIONS 
### 1. TRADITIONAL BUILD 
* "Traditional" hosting solutions like OVH, 1and1, or Gandhi where you have to upload files manually by using an FTP client 
* first need to build project:
    - run `npm run build` in the terminal
    - upload all files from the `/dist/`
### 2. VERCEL 
* more appropriate solution 
* "modern" hosting solution 
* continuous integration (automisation of testing, deployment, etc.)
* developer friendly
* easy setup
* for complex or simple projects
### ALTERNATIVES
* `Netlify`
* `GitHub Pages`

## USING VERCEL
* create an account
* when using `GitHub` Vercel will automatically fetch repos
* help setup live version 
* automatically updates when you push new versions on the repo

### ADD VERCEL TO PROJECT
* available as an `NPM module`
* install as globally on compy or as dependency on your project
* adding it to project:
    - `npm install vercel`
* in `package.json` in the `"scripts"` property, ass a new script named `"deploy"`:
    ```
    {
        "scripts": {
            "deploy": "vercel --prod"
        },
    }
    ```
* if you use the `"vercel"` command without `--prod` the code will be published on a preview URL

### DEPLOY FOR THE FIRST TIME
* in terminal run `npm run deploy` and follow steps 

### FURTHER SETTINGS
* many features:
    - see a preview of project
    - get info abou the latest builds
    - change deployment prefrences
    - see potential errors
    - etc. 
* can add custom domain 