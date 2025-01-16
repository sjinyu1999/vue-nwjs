# vue-nwjs
node版本   20+
应用到nwjs时，首先需要build   
```pnpm build```
然后将生成的 dist 文件里的内容放到 nwjs-app 的根目录下，然后运行 
```npx nw .```即可

# 打包应用
首先安装nw-builder ```npm install -g nw-builder```
然后在你的nwjs-app文件夹中运行以下命令来打包应用：
```nwbuild -p win64,win32,osx64,linux64 .```
生成 package.json ```npm init -y```
下载 ```npm install nw --save-dev``` 或者直接在官网下载：https://dl.nwjs.io/v0.94.1/nwjs-sdk-v0.94.1-win-x64.zip
然后将打包的 dist 文件夹内容复制到下载的 nw 文件夹中，复制根目录中的 package.json 到 nw 文件夹中，然后运行 nw 文件夹中的 nw.exe 即可
This template should help get you started developing with Vue 3 in Vite.

## Recommended IDE Setup

[VSCode](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur).

## Type Support for `.vue` Imports in TS

TypeScript cannot handle type information for `.vue` imports by default, so we replace the `tsc` CLI with `vue-tsc` for type checking. In editors, we need [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) to make the TypeScript language service aware of `.vue` types.

## Customize configuration

See [Vite Configuration Reference](https://vite.dev/config/).

## Project Setup

```sh
pnpm install
```

### Compile and Hot-Reload for Development

```sh
pnpm dev
```

### Type-Check, Compile and Minify for Production

```sh
pnpm build
```

### Run Unit Tests with [Vitest](https://vitest.dev/)

```sh
pnpm test:unit
```

### Lint with [ESLint](https://eslint.org/)

```sh
pnpm lint
```
