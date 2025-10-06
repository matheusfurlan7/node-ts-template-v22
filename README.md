# node-ts-template-v22
Base template Node.js + TypeScript with lint, prettier, husky, vitest, CI and Docker.

### Index 
- [Title and description](#node-ts-template-v22)
- [Index](###Index)
- [Tools](###Tools)
- [Scripts](###Scripts)

### Tools
- **TypeScript:** [https://github.com/microsoft/TypeScript](https://github.com/microsoft/TypeScript)
- **tsc-alias:** [https://github.com/justkey007/tsc-alias](https://github.com/justkey007/tsc-alias)
- **ts-node-dev:** [https://github.com/wclr/ts-node-dev](https://github.com/wclr/ts-node-dev)

### Scripts

To run the project, use the following commands:

**1. Install dependencies**
```bash
npm install
```
To install all dependencies listed in the `package.json` file

**2. Developer mode**
```bash
npm run dev
```
Start the server in developer mode with `ts-node-dev`. It automatically restarts when a change is detected and rebuilds only what's necessary to speed up development.

**3. Compile for production**
```bash
npm run build
```
Compiles TypeScript files to JavaScript (`tsc`) and then rewrites the path aliases in the output files (`tsc-alias`) so that Node.js can run correctly