# Vue 3 + Vite
- 项目创建 node 版本 v8.19.1
- 项目创建快速命令：npm create vite@latest bs-page -- --template vue
- npm install
- npm run dev

# Tailwind css
- npm install -D tailwindcss
- npx tailwindcss init
- 安装完毕后，安装插件 PostCss Language Support
- 一步到位的 TailWind CSS 支持：Tailwind CSS IntelliSense

# 终极解决
- npm install -D tailwindcss postcss autoprefixer
- 配置tailwind.config.js
```   
/** @type {import("tailwindcss").Config} */
export default {
  content: ['./index.html', './src/**/*.{vue,js,ts,jsx,tsx}'],
  theme: {
    extend: {},
    fontFamily: {
    
    },
  },
  plugins: [],
};

```

- 新建 postcss.config.js  
``` 
module.exports = {
  plugins: {
    tailwindcss: {},
    autoprefixer: {},
  },
};

```
- package.json中配置
```  
 "postcss": {
    "plugins": {
      "tailwindcss": {},
      "autoprefixer": {}
    }
  }
```
- 最后一步，某个目录新建一个 css，在main.js中引入 
```  
@tailwind base;
@tailwind components;
@tailwind utilities;

```
 大功告成！