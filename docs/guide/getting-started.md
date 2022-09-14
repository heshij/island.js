# Getting Started

## Why Island?

🏝️ Island(`/ˈaɪlənd/`) is a static site generator that builds on top of Vite and Mdx. It is designed to be simple, powerful, and performant. It is built to help you focus on writing and deployed with minimum configuration.It has the following features:

- **Fast**: Island is built on top of Vite, which is a modern build tool that aims to provide a faster and leaner development experience.
- **Flexible**: It has internal Mdx language support, which is a powerful way to write content. You can write, import and use React components in Markdown file.
- **Performant**: It is designed to be [island architecture](https://jasonformat.com/islands-architecture/), which means less javascript bundle, partial hydration and better performance about FCP, TTI.

## Quick Start

First, you can use `npm init -y` to init a new project.Then you can install Island with npm, yarn or pnpm:

```bash
// npm
npm install island-ssg
// yarn
yarn add island-ssg
// pnpm
pnpm add island-ssg
```

Then you can create file:

```bash
`mkdir docs && echo '# Hello World' > docs/index.md`
```

And then you can add the following scripts in `package.json`:

```json
// package.json
{
  "scripts": {
    "dev": "island dev docs",
    "build": "island build docs",
    "preview": "island start docs"
  }
}
```

Serve the documentation site in the local server.

```bash
yarn dev
```

Island will start a development server at http://localhost:5173.