# node-ts-template-v22

Base template Node.js + TypeScript with lint, prettier, husky, vitest, CI and Docker.

## Index

- [Title and description](#node-ts-template-v22)
- [Index](#index)
- [Tools](#tools)
- [Scripts](#scripts)

## Tools

- **TypeScript:** [https://github.com/microsoft/TypeScript](https://github.com/microsoft/TypeScript)
- **tsc-alias:** [https://github.com/justkey007/tsc-alias](https://github.com/justkey007/tsc-alias)
- **ts-node-dev:** [https://github.com/wclr/ts-node-dev](https://github.com/wclr/ts-node-dev)
- **ESLint:** [https://github.com/eslint/eslint](https://github.com/eslint/eslint)
- **Prettier:** [https://github.com/prettier/prettier](https://github.com/prettier/prettier)

## Scripts

To run the project, use the following commands:

**Install dependencies**

```bash
npm install
```

To install all dependencies listed in the `package.json` file

**Developer mode**

```bash
npm run dev
```

Start the server in developer mode with `ts-node-dev`. It automatically restarts when a change is detected and rebuilds only what's necessary to speed up development.

**Compile for production**

```bash
npm run build
```

Compiles TypeScript files to JavaScript (`tsc`) and then rewrites the path aliases in the output files (`tsc-alias`) so that Node.js can run correctly

**Code Quality**

```bash
npm run lint
```

Check if there is any inconsistency in the code, for example, unused variable

```bash
npm run lint:fix
```

check for inconsistencies and adjust the file

```bash
npm run format
```

Check and adjust spacing and style inconsistencies in the project

```bash
npm run format:check
```

Check **(not adjust)** spacing and style inconsistencies in the project
