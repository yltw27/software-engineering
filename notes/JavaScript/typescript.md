# TypeScript

[Intermediate React, V3 on FrontendMaster](https://frontendmasters.com/courses/intermediate-react-v3) (There's a section for TypeScript)

## Introduction

- TypeScript is a type checker for JavaScript (an untyped language)

- TypeScript forces you to be more defensive while coding

## Set up

- Install TypeScript

    ```bash
    npm i -D typescript
    ```

- Init command gives you a configuration file named `tsconfig.json`

    ```bash
    npx tsc --init
    ```

- Install the types if the framework (e.g. React) you are using is not written in TypeScript

    ```bash
    npm i -D @types/react @types/react-dom @types/react-router-dom
    ```

### TypeScript + ESLint

1. `npm i -D eslint-import-resolver-typescript @typescript-eslint/eslint-plugin @typescript-eslint/parser`

2. Check your rules in `.eslintrc.json`. You can add this:

    ```JSON
    {
        "extends": [
            "plugin:@typescript-eslint/recommended",
            "plugin:@typescript-eslint/recommended-requiring-type-checking"
        ],
        "plugins": [
            "@typescript/eslint"
        ],
        "parser": "@typescript/eslint-parser",
        "parserOptions": {
            "project": "./tsconfig.json"
        },
        "settings": [
            "import/parsers": {
                "@typescript-eslint/parser": [ ".ts", ".tsx" ]
            }
            "import/resolver": {
                "typescript": {
                    "alwaysTryTypes": true
                }
            }
        ],
        // ...
    }
    ```

3. `npm run lint` shows linting errors or use `npm run lint:fix` to fix the errors automatically

### Migration

- Rename your `.js/.jsx` files to `.ts/.tsx`
 