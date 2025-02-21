# Next.js 15 Build Error: Missing export 'default'

This repository demonstrates a bug encountered in Next.js 15 where the build process fails with an error related to a missing default export, even when the export is correctly defined.

## Bug Description

When building a Next.js 15 application, an error is thrown indicating that a default export is missing from a component file. However, upon inspection, the default export is clearly present in the code. This issue only manifests during the build process and doesn't prevent the application from running in development mode. 

## How to Reproduce

1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install` to install dependencies.
4. Run `npm run build` to trigger the build process.  You will see the error.

## Solution
The solution involves ensuring that your Next.js configuration is correctly set up, especially when using features like `app` directory. The `pages` directory and `app` directory structures have different requirements. Making sure exports are correct within those separate contexts is crucial. The solution provided ensures this is handled correctly.