- Tailwind css In Vue (Visual Studio Code)

```sh
npm create vue@latest
cd vue-project
npm install
npm install -D tailwindcss@latest postcss@latest autoprefixer@latest
npx tailwindcss init
```

$ tailwind.config.js in vue-project
```sh
/** @type {import('tailwindcss').Config} */
export default {
  purge: ['./index.html', './src/**/*.{vue,js,ts,jsx,tsx}'],
  darkMode: false,
  theme: {
    extend: {},
  },
  plugins: [],
}
```

$ Make new file postcss.config.js inside same folder with tailwind.config.js
```sh
export default {
    plugins: {
      tailwindcss: {},
      autoprefixer: {},
    },
  }
```

$ Make tailwind.css inside src
```sh
@tailwind base;
@tailwind components;
@tailwind utilities;
```

$ go to main.js
```sh
import './tailwind.css'
```

$ to run the website
```sh
npm run dev
```

#####################################################################
- Second Method

$ Vsc terminal
```sh
npm create vite@latest my-project -- --template vue
cd my-project
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p

/** @type {import('tailwindcss').Config} */
export default {
  content: [
    "./index.html",
    "./src/**/*.{vue,js,ts,jsx,tsx}",
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}

@tailwind base;
@tailwind components;
@tailwind utilities;
npm run dev
```

#####################################################################
- Git Bash

$ cd to the folder to upload
```sh
git init
git add .
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/..../....
git push -u origin main
```
```sh
				<!--'/Product-preview/' -->
$ got to vite.config.js in folder add {base: '/<REPO NAME>/',} 
npm run build 
git add dist -f
git commit -m "adding dist"
git subtree push --prefix dist origin gh-pages

got to github main -> Branches -> gh-pages
```

#####################################################################
- Tailwind Install in HTML

```sh
npm install -D tailwindcss
npx tailwindcss init
```
$ Inside tailwind.config.js
```sh
content: ["./index.html"],
```
# add new file in folder src -> input.css 
```sh
@tailwind base;
@tailwind components;
@tailwind utilities;
```
```sh
npx tailwindcss -i ./src/input.css -o ./src/output.css --watch
```
$ in HTML
```sh
<link href="./src/output.css" rel="stylesheet">
```
#####################################################################
- Git Terminal VSC
```sh
git init 
git add origin
git remote add origin https:/github.com/.....
git add -A
git commit -m "Initial commit"
git push origin master
```

#####################################################################


Welcome any suggestions for improvement. Thank You.
