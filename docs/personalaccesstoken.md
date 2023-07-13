# Personal access token for the GitHub registry

## Content

- [Personal access token for the GitHub registry](#personal-access-token-for-the-github-registry)
  - [Content](#content)
  - [Purpose for personal access token](#purpose-for-personal-access-token)
  - [Create an personal access token on GitHub](#create-an-personal-access-token-on-github)
  - [Login into Simatic-Ax registry](#login-into-simatic-ax-registry)
    - [Login via CLI](#login-via-cli)
    - [Login via AX Code UI /Web or local IDE)](#login-via-ax-code-ui-web-or-local-ide)
  - [Workspace settings to access the GitHub registry](#workspace-settings-to-access-the-github-registry)

## Purpose for personal access token

To be able to consume some packages from the `simatic-ax` group, you need to login into the registry.

## Create an personal access token on GitHub

To create an personal access on GitHub token follow this [link](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)

> It's ***very*** important that you check the checkbox `write:packages`
>
> ![image](images/readpackage.png)
>
> For security reasons, your token should be expire after wa while (by default it's 30 days).
>
> Remember this token. You'll need it for the login in the next step.

## Login into Simatic-Ax registry

### Login via CLI

To login via CLI you've to enter the following command. You've to replace `<your personal access token>` by your on Github created access token.

```cli
apax login --registry https://npm.pkg.github.com/ --password <your personal access token>
```

### Login via AX Code UI /Web or local IDE)

To login into the GitHub registry for Simatic AX within your IDE (Web or local AX Code) follow this steps:

1. select the file `apax.yml`, click the right mouse button and select `Login to registry`

    ![drawing](images/apax_login.png)  

1. Enter the GitHub URL

     ![drawing](images/github_url.png)  

    ```url
    https://npm.pkg.github.com/
    ```

1. Leave the user name field empty and press `Enter`

    ![drawing](images/enter.png)  

1. Enter your personal access token from GitHub with `Strg+V`

    ![drawing](images/token.png)  

Now you're able to install all dependencies to develop on your library.

## Workspace settings to access the GitHub registry

To access the GitHub registry from your workspace, you've to announce it in the apax.yml.

Please enter the following code into your apax.yml:

```yml
registries:
  '@simatic-ax': 'https://npm.pkg.github.com/'
```
