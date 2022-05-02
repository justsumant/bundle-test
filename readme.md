https://www.youtube.com/watch?v=XHQi5a0TmMc
https://dev.to/alexeagleson/how-to-create-and-publish-a-react-component-library-2oe

npm init
create src/components/button/Button.tsx
export from src/components/button , src/components and src
npm install react typescript @types/react --save-dev
npx tsc --init
add following in tsconfig.json -> compiler options
"skipLibCheck": true /_ Skip type checking all .d.ts files. _/,
"jsx": "react",
"module": "ESNext",
"declaration": true,
"declarationDir": "types",
"sourceMap": true,
"outDir": "dist",
"moduleResolution": "node",
"allowSyntheticDefaultImports": true,
"emitDeclarationOnly": true

webpack is specially for bundeling the big modules to simple project (static files) which browser could understand while rollup is specially used for bundeling libraries. same can be achieved using webpack too but with different efficiency.

npm install rollup @rollup/plugin-node-resolve @rollup/plugin-commonjs @rollup/plugin-typescript rollup-plugin-dts --save-dev
create rollup.config.js
