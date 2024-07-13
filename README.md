# 🚀 TypeScript Lambda Boilerplate

This is a TypeScript Lambda template that helps you quickly start developing your AWS Lambda functions. It uses the Serverless Framework for easy deployment and local development.

## 🛠️ Technologies Used

- 📗 Node.js (v20.x)
- 📘 TypeScript
- ☁️ AWS Lambda
- 🔧 Serverless Framework
- 📦 esbuild (for bundling)

## 📚 Dependencies

### 🏭 Production Dependencies

This project doesn't have any production dependencies. All required AWS SDK modules are available in the Lambda runtime environment.

### 🔬 Development Dependencies

- `@types/aws-lambda`: TypeScript definitions for AWS Lambda
- `@types/node`: TypeScript definitions for Node.js
- `esbuild`: JavaScript bundler and minifier
- `serverless`: Serverless Framework CLI
- `serverless-esbuild`: Serverless plugin for using esbuild
- `serverless-offline`: Serverless plugin for local development
- `typescript`: TypeScript compiler

## 📁 Project Structure

```sh
├── serverless.yml
├── package.json
├── pnpm-lock.yaml
├── README.md
├── .npmrc
├── src
│   └── handler.ts
└── tsconfig.json
```

## 🚀 Setup

1. Clone this repository
2. Install dependencies:

```sh
pnpm install
```

## 🖥️ Usage

### 🏠 Local Development

To run the function locally:

```sh
pnpm start
```

This will start the Serverless Offline server on port 9000.

### 🚀 Deployment

To deploy the function to AWS:

```sh
pnpm run deploy
```

### 🗑️ Removal

To remove the deployed function from AWS:

```sh
pnpm run remove
```

## ⚙️ Configuration

- The `serverless.yml` file contains the Serverless Framework configuration.
- The `tsconfig.json` file contains the TypeScript compiler options.
- The `package.json` file lists the project dependencies and scripts.

## 🎯 Function

The boilerplate includes a simple "hello world" function in `src/handler.ts`. You can modify this function or add new functions as needed.

## 📜 License

This project is licensed under the ISC License. See the [LICENSE](LICENSE) file for details.
