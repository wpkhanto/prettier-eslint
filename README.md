# Project Setup

```bash
npm install -D eslint eslint-config-airbnb eslint-config-prettier eslint-plugin-import eslint-plugin-jsx-a11y eslint-plugin-node eslint-plugin-prettier eslint-plugin-react prettier
```

## Step 1: Prettier Configuration

1. Create a `.prettierrc` file in your project directory with the following content:

```json
{
    "singleQuote": true
}
```

## Step 2: ESLint Configuration

1. Create a `.eslintrc.json` file with the following configuration:

```json
{
    "extends": ["airbnb", "prettier", "plugin:node/recommended"],
    "plugins": ["prettier"],
    "rules": {
        "prettier/prettier": "error",
        "spaced-comment": "off",
        "no-console": "warn",
        "consistent-return": "off",
        "func-names": "off",
        "object-shorthand": "off",
        "no-process-exit": "off",
        "no-param-reassign": "off",
        "no-return-await": "off",
        "no-underscore-dangle": "off",
        "class-methods-use-this": "off",
        "prefer-destructuring": ["error", { "object": true, "array": false }],
        "no-unused-vars": ["error", { "argsIgnorePattern": "req|res|next|val" }]
    }
}
```