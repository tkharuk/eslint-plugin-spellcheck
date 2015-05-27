# eslint-plugin-spellcheck
[eslint](http://eslint.org) plugin to spell check words on identifiers, Strings and comments of javascript files.

## Usage in a project

1. Install `eslint-plugin-spellcheck` as a dev-dependency:

    ```shell
    npm install --save-dev eslint-plugin-spellcheck
    ```

2. Enable the plugin by adding it to your `.eslintrc`:

    ```yaml
    plugins:
      - spellcheck
    ```
3. You can also configure these rules in your `.eslintrc`. All rules defined in this plugin have to be prefixed by 'spellcheck/'

    ```yaml
    plugins:
      - spellcheck
    rules:
      - spellcheck/spell-strings: 0
    ```

## Usage globally

1. Install `eslint-plugin-spellcheck` as a global package:

    ```shell
    npm install -g eslint-plugin-spellcheck
    ```

2. Enable the plugin by adding it to your `eslint.json`:

    ```json
    "plugins": [
       "spellcheck"
   ],
   "rules": {
       "spellcheck/spell-strings": 1
       }
    ```

## Rules

| Name  | Description | Default Configuration |
| ------------- | ------------- | ------------- |
| spell-comments  | Check spelling inside js comments | 'spell-comments': 1 |
| spell-strings | Check spelling on each word in strings | 'spell-strings': 1 |
| spell-identifiers | Check spelling on identifiers, separatesd words if camelCased or snake_cased | 'spell-identifiers': 1 |
