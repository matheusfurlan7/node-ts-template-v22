![Node.js v22](https://img.shields.io/badge/Node.js-v22-43853D?style=for-the-badge&logo=node.js&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![ESLint](https://img.shields.io/badge/ESLint-4B32C3?style=for-the-badge&logo=eslint&logoColor=white)
![Prettier](https://img.shields.io/badge/Prettier-FF69B4?style=for-the-badge&logo=prettier&logoColor=white)
![Vitest](https://img.shields.io/badge/Vitest-F7B93E?style=for-the-badge&logo=vitest&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-0db7ed?style=for-the-badge&logo=docker&logoColor=white)

# node-ts-template-v22

Base template Node.js + TypeScript with lint, prettier, husky, vitest, CI and Docker.

## Index

- [Title and description](#node-ts-template-v22)
- [Index](#index)
- [Technologies](#technologies)
- [Tools](#tools)
- [Scripts](#scripts)
- [Docker](#docker)
- [Contact](#contact)

## Technologies

This project was built with the following core technologies:

<br>

<p align="left">
  <img src="https://skillicons.dev/icons?i=nodejs,typescript,vitest,docker" />
</p>

## Tools

- [**TypeScript**](https://github.com/microsoft/TypeScript) - Put typing in JavaScript.
- [**tsc-alias**](https://github.com/justkey007/tsc-alias) - Fix import path to absolute path.
- [**Nodemon**](https://github.com/remy/nodemon) - Automatically restarts the server after changing the code.
- [**ts-node**](hhttps://github.com/TypeStrong/ts-node) - Run TypeScript files directly in Node.js without the need for manual compilation.
- [**ESLint**](https://github.com/eslint/eslint) - Identifies and reports problematic patterns in code, ensuring quality and standardization
- [**Prettier**](https://github.com/prettier/prettier) - Opinionated code formatter that ensures consistent style across the project.
- [**Husky**](https://github.com/typicode/husky) - Facilitates the use of Git Hooks to run scripts before a commit or push.
- [**Lint-staged**](https://github.com/lint-staged/lint-staged) - Runs commands (linters) only on files that have been changed and added to the next commit.
- [**Vitest**](https://github.com/vitest-dev/vitest) - An ultra-fast testing framework for JavaScript and TypeScript, focused on performance.
- [**Docker**](https://www.docker.com/) - The open source platform for developing, shipping, and running containerized applications.

## NVM

```bash
nvm use
```

Adjust the node version to match the project.

## Scripts

To run the project, use the following commands:

### Basic

**Install dependencies**

```bash
npm install
```

To install all dependencies listed in the `package.json` file

### Run code

**Developer mode**

```bash
npm run dev
```

Start the server in developer mode with `nodemon`. It automatically restarts when a change is detected and rebuilds only what's necessary to speed up development.

**Compile for production**

```bash
npm run build
```

Compiles TypeScript files to JavaScript (`tsc`) and then rewrites the path aliases in the output files (`tsc-alias`) so that Node.js can run correctly

### **Code Quality**

**Husky**

```bash
npm run prepare
```

To prepare Husky to work and check files pre-commit

**ESLint**

```bash
npm run lint
```

Check if there is any inconsistency in the code, for example, unused variable

```bash
npm run lint:fix
```

Check for inconsistencies and adjust the file

**Prettier**

```bash
npm run format
```

Check and adjust spacing and style inconsistencies in the project

```bash
npm run format:check
```

Check **(not adjust)** spacing and style inconsistencies in the project

**Vitest**

```bash
npm run test
```

Run the automated test and wait for new tests, or adjust the code to run the tests that reported an error.

```bash
npm run test:run
```

Run the automated test only once.

```bash
npm run test:coverage
```

Run the automated test and show the percentage of files covered

## Docker

This project includes two Docker environments: one for **development** (with hot reload) and another for **production** (optimized and lightweight).

Make sure you have Docker installed and running before executing the commands below.

**Development**

Build and run the container in development mode, with automatic reload via `nodemon`.

```bash
# Build image
docker build -f Dockerfile.dev -t ts-template-dev .

# Run container with live reload and local volume
docker run -it -v .:/app -p 3000:3000 ts-template-dev
```

Build and run the container in development mode, with automatic reload via `nodemon`.

**Production**

```bash
# Build optimized image
docker build -f Dockerfile.prod -t ts-template-prod .

# Run container in detached mode
docker run -d -p 3000:3000 ts-template-prod
```

Build and run the container in **production mode**, optimized for size and performance.

## Contact

Connect with me:

<a href="https://github.com/matheusfurlan7" target="_blank">
  <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" />
</a>
<a href="https://www.linkedin.com/in/matheusfurlan7" target="_blank">
  <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
</a>
