# sb-styles

A styling library for Sunbird projects that provides SCSS components and stylesheets.

### Local Development

1. Fork the repository on GitHub

2. Clone your fork:

``` 
 git clone https://github.com/your-username/sb-styles.git

cd sb-styles
```
3. Install dependencies:

```
npm i --legacy-peer-deps
```
4. To run the project
```
npm run build-css
```

### This project uses GitHub Actions for automated builds and security scanning.

## PR Build
1. Performs static code analysis with CodeQL for security vulnerabilities
1. Compiles SCSS files to CSS

1. Creates a distributable npm package

### How It Works

When a PR is opened, the workflow:

1. Sets up the Node.js environment
1. Installs dependencies
1. Builds the project
1. Runs security scans
1. Packages the library

## Release process

### Prerequisite
- Set the `NPM_TOKEN` secret in your GitHub repository settings

When tags are pushed, the workflow automatically:

1. Builds the package
1. Publishes to NPM registry

## Link

1. [NPM Package](https://www.npmjs.com/package/@project-sunbird/sb-styles)