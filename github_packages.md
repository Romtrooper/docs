# Managing Packages

[Official Github Packages doumentation](https://help.github.com/en/packages)

1. Create a [Github Token](https://github.com/settings/tokens)
1. Authenticate using your access token

# Installation and usage

## In your project

Add a `.npmrc` file in your root folder

```
registry=https://npm.pkg.github.com/{github_repo}
```

```
npm install @{owner}/{package_name}
```

### Installing for CI (continuous integration)
 
#### Circle CI

In your `config.yml` before running `npm install` set:

 ```yaml
steps:
    - run: npm set //npm.pkg.github.com/:_authToken=${GITHUB_TOKEN}
 ```

Then go to you project settings in [app.circleci.com](https://app.circleci.com/projects) in __Environment Variables__ en create a variable name `GITHUB_TOKEN` with the value of the token.
