# Contributing to LayoutContainer Component

Here are some guidelines to help you get started.

## Table of Contents

1. [Getting Started](#getting-started)
2. [Development](#development)
3. [Code Style](#code-style)
4. [Submitting Changes](#submitting-changes)

## Getting Started

1. Clone the repository to your local machine:
    ```sh
    git clone https://github.com/sitecorelabs/sitecore-xmcloud-components-layout-container
    ```
2. Navigate to the project directory:
    ```sh
    cd sitecore-xmcloud-components-layout-container
    ```
3. Install the dependencies:
    ```sh
    npm install
    ```

## Development

The main component you will be working on is located in the `src/component/layout-container` directory.

- `src/component/layout-container/LayoutContainer.tsx`: Main React component.
- `src/component/layout-container/index.scss`: Main SCSS file for styling.
- `src/component/layout-container/_functions.scss`: SCSS functions.
- `src/component/layout-container/_variables.scss`: SCSS variables.


## Code Style

We use ESLint and Prettier to maintain code quality and consistency. Please make sure your code adheres to the style guidelines by running:
```sh
npm run lint
```

## Submitting Changes

1. Create a new branch for your feature or bugfix:
    ```sh
    git checkout -b feature/your-feature-name
    ```
2. Make your changes and commit them with a clear and descriptive commit message:
    ```sh
    git commit -m "Add feature: your feature description"
    ```
3. Push your changes to repository:
    ```sh
    git push origin feature/your-feature-name
    ```
4. Open a pull request against the main repository.

Thank you for your contributions!
```
