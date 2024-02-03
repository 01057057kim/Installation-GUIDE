-Tailwind css In Vue (Visual Studio Code)

npm create vue@latest
{
cd vue-project
npm install
}

npm install -D tailwindcss@latest postcss@latest autoprefixer@latest
npx tailwindcss init

$ tailwind.config.js in vue-project
{

/** @type {import('tailwindcss').Config} */
export default {
  purge: ['./index.html', './src/**/*.{vue,js,ts,jsx,tsx}'],
  darkMode: false,
  theme: {
    extend: {},
  },
  plugins: [],
}

}

$ make new file postcss.config.js inside same folder with tailwind.config.js
{

export default {
    plugins: {
      tailwindcss: {},
      autoprefixer: {},
    },
  }
  
}

Make tailwind.css inside src
{

@tailwind base;
@tailwind components;
@tailwind utilities;

}

go to main.js
{
import './tailwind.css'
}

npm run dev
#####################################################################
Git Bash

cd to folder to upload

git init
git add .
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/..../....
git push -u origin main
					<!--'/Product-preview/' -->
got to vite.config.js in folder add {base: '/<REPO NAME>/',} 
npm run build 
git add dist -f
git commit -m "adding dist"
git subtree push --prefix dist origin gh-pages

got to github main -> Branches -> gh-pages

#####################################################################

-Tailwind Install in HTML

npm install -D tailwindcss
npx tailwindcss init
content: ["./index.html"],
new file in folder src -> input.css 
{
@tailwind base;
@tailwind components;
@tailwind utilities;
}

npx tailwindcss -i ./src/input.css -o ./src/output.css --watch

<in HTML>
<link href="./src/output.css" rel="stylesheet">

#####################################################################
-Git Terminal VSC

git init 
git add origin
git remote add origin https:/github.com/.....
git add -A
git commit -m "Initial commit"
git push origin master

#####################################################################


Welcome any suggestions for improvement. Thank You.
