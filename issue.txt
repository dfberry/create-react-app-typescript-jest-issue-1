# Jest test run finds no test

## To reproduce

1. create app

    ```
    npx create-react-app my-app --template typescript
    ```

1. run tests

    ```
    cd my-app && npm run test
    ```

## Run results in terminal

No tests found related to files changed since last commit.
Press `a` to run all tests, or run Jest with `--watchAll`.

Watch Usage
 › Press a to run all tests.
 › Press f to run only failed tests.
 › Press q to quit watch mode.
 › Press p to filter by a filename regex pattern.
 › Press t to filter by a test name regex pattern.
 › Press Enter to trigger a test run.

 ## Fix

To fix this issue ([fix branch](https://github.com/dfberry/create-react-app-typescript-jest-issue-1/tree/fix)):

1. Create `__tests__` directory under `src`.
1. Move `App.test.tsx` into that directory.
1. Change `App.test.tsx` import statement:

    ```
    import App from '../App';
    ```

