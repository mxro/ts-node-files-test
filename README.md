# ts-node-files-test

This repository contains a project testing if the `--files` directive of `ts-node` works.

## Usage

```
npm i
npm run node
```

## Setup

The project contains both an `index.ts` file:

```typescript
import styles from './index.css';

console.log("I'm in index.ts and I got the following styles:", styles);
```

That imports the CSS file `index.css`. There is also a `typings.d.ts` file that contains a module declaration:

```typescript
declare module '*.css';
```

## Findings

The project compiles successfully using `tsc` but does not run when using `ts-node`.
