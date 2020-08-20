# Setup for Formatting Code Automatically

## `husky` + `lint-staged` + `prettier`

* `husky` makes it possible to use githooks as if they are npm scripts. https://github.com/typicode/husky
* `lint-staged` allows us to run scripts on staged files in git. https://github.com/okonet/lint-staged
* `prettier` is the JavaScript formatter we will run before commits. https://github.com/prettier/prettier

## Resources
* https://create-react-app.dev/docs/setting-up-your-editor/#formatting-code-automatically
* https://prettier.io/docs/en/install.html

## How It's Set Up

Basically followed the create-react-app instruction, and tweaked some parts based on the prettier doc.

* Install exact version of prettier for consistent formatting for everyone in the project.
* Install the packages in devDependencies.
* Add `.prettierrc.json` and `.prettierignore`
* `eslint-config-prettier` doesn't seem to be needed for `create-react-app` project.
* `lint-staged` config in the create-react-app instruction works better. 
  * `eslint --fix` fails in a create-react-app project. Also it shouldn't be needed when using Prettier for formatting.
  * Whitelisting file types work better than blacklisting in `.prettierignore`


---

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `yarn start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

### `yarn test`

Launches the test runner in the interactive watch mode.<br />
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `yarn build`

Builds the app for production to the `build` folder.<br />
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br />
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `yarn eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: https://facebook.github.io/create-react-app/docs/code-splitting

### Analyzing the Bundle Size

This section has moved here: https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size

### Making a Progressive Web App

This section has moved here: https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app

### Advanced Configuration

This section has moved here: https://facebook.github.io/create-react-app/docs/advanced-configuration

### Deployment

This section has moved here: https://facebook.github.io/create-react-app/docs/deployment

### `yarn build` fails to minify

This section has moved here: https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify
