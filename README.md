# Host Client Side Shiny Apps On Github For Free

## Introduction

This is a simple guide to hosting client side web apps on github for free. This is a great way to host your web apps for free and also to learn about git and github.

## Steps

1. Create a github account if you don't already have one.
2. Create a new repository on github. Name it whatever you want.
3. Clone the repository to your local machine.
4. Add your shiny app files to the `src` folder.
5. Commit and push your changes to github.
6. Set up github pages for your repository. 
7. Go to settings and scroll down to the github pages section. 
8. Select the master branch as the source and click save. 

You should see a link to your shiny app. It may take a few minutes for the link to work.

## Example

Here is an example of a shiny app hosted on github pages: https://joshua-silver.shinyapps.io/iris/

## FAQ
> Why does is take so long to load?

As the shiny app is running in the client's browser, the app's dependencies must be downloaded to the client's browser. This can take a while depending on the size of the app and the client's internet connection. However, once the dependencies are downloaded once they will be cached in the client's browser and the app will load much faster in the future.

> Why does the app not work?

Client-side shiny apps only work with pre-compiled dependencies. This means that you cannot use packages that require compilation such as `sf` and `rstan`. At list of packages that can be used can be found at [https://repo.r-wasm.org/](https://repo.r-wasm.org/).