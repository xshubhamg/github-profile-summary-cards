<div align="center">
   <h1>GitHub Profile Summary Cards</h1>


   [繁體中文](./docs/README.zh-tw.md)
   <p>
      A tool to generate your github summary card for profile README. Inspired by <a href=https://github.com/tipsy/profile-summary-for-github>profile-summary-for-github</a>
   </p>
   <p>
      :star: This repo is just for fun, feel free to contribute! :star:
   </p>
   <p align="center">
      <a href="https://github.com/xshubhamg/github-profile-summary-cards/stargazers">
      <img alt="Stargazers" src="https://img.shields.io/github/stars/xshubhamg/github-profile-summary-cards?style=for-the-badge&logo=github&color=f4dbd6&logoColor=D9E0EE&labelColor=302D41"></a>
      <a href="https://github.com/xshubhamg/github-profile-summary-cards/releases/latest">
      <img alt="Releases" src="https://img.shields.io/github/release/xshubhamg/github-profile-summary-cards.svg?style=for-the-badge&logo=semantic-release&color=f5bde6&logoColor=D9E0EE&labelColor=302D41"/></a>
      <a href="https://www.conventionalcommits.org/en/v1.0.0/">
      <img alt="conventionalcommits" src="https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?style=for-the-badge&logo=conventionalcommits&color=ee99a0&logoColor=D9E0EE&labelColor=302D41"></a>
      <a href="https://github.com/xshubhamg/github-profile-summary-cards/actions/workflows/github-action.yml">
      <img alt="testandlint" src="https://img.shields.io/github/actions/workflow/status/xshubhamg/github-profile-summary-cards/test-and-lint.yml?branch=main&label=Test%20and%20Lint&style=for-the-badge&color=a6da95"></a>
   </p>
</div>

<div align="center">
<p>
<a href="https://github-profile-summary-cards.vercel.app/demo.html">Get your own cards now!!</a>
</p>


![](https://raw.githubusercontent.com/xshubhamg/xshubhamg/master/profile-summary-card-output/solarized/0-profile-details.svg)
![](https://raw.githubusercontent.com/xshubhamg/xshubhamg/master/profile-summary-card-output/solarized/1-repos-per-language.svg)
![](https://raw.githubusercontent.com/xshubhamg/xshubhamg/master/profile-summary-card-output/solarized/2-most-commit-language.svg)
![](https://raw.githubusercontent.com/xshubhamg/xshubhamg/master/profile-summary-card-output/solarized/3-stats.svg)
![](https://raw.githubusercontent.com/xshubhamg/xshubhamg/master/profile-summary-card-output/solarized/4-productive-time.svg)

</div>

## Themes

|   |   |   |   |   |
|:---:|:---:|:---:|:---:|:---:|
|default|2077|dracula|github|github_dark|
|![](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=xshubhamg&theme=default)|![](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=xshubhamg&theme=2077)| ![](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=xshubhamg&theme=dracula)|![](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=xshubhamg&theme=github)|![](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=xshubhamg&theme=github_dark)|
|gruvbox|monokai|nord_bright|nord_dark|radical|
|![](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=xshubhamg&theme=gruvbox)|![](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=xshubhamg&theme=monokai)| ![](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=xshubhamg&theme=nord_bright)|![](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=xshubhamg&theme=nord_dark)  |![](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=xshubhamg&theme=radical)|
|solarized|solarized_dark|tokyonight|vue|zenburn|
|![](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=xshubhamg&theme=solarized)|![](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=xshubhamg&theme=solarized_dark)| ![](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=xshubhamg&theme=tokyonight)|![](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=xshubhamg&theme=vue)  |![](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=xshubhamg&theme=zenburn)|
|transparent|catppuccin_frappe|catppuccin_mocha|   |   |
|![](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=xshubhamg&theme=transparent)|![](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=xshubhamg&theme=catppuccin_frappe)|![](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=xshubhamg&theme=catppuccin_mocha)|   |   |

[More themes](https://github.com/xshubhamg/github-profile-summary-cards-example/tree/master/profile-summary-card-output)

## How to use (API)

You can use the public API hosted on Vercel, or [deploy your own instance](deployment.md).

### Profile details card
![](http://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=xshubhamg&theme=nord_bright)

`http://github-profile-summary-cards.vercel.app/api/cards/profile-details?username={username}&theme={theme_name}`
- Accept url parameters
  - theme
    - Theme name
  - username
    - Username
### Top languages used in repository card
![](http://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=xshubhamg&theme=nord_bright)

`http://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username={username}&theme={theme_name}&exclude={exclude}`
- Accept url parameters
  - theme
    - Theme name
  - username
    - Username
  - exclude:
    - A comma separated list of languages to exclude, e.g., exclude=java,rust,jupyter%20Notebook
      - You can represent a space in the language list by using '%20' when you want to include a space.
    - You can found the supported languages in [here](https://github.com/github/linguist/blob/master/lib/linguist/languages.yml)

### Top languages in commits card
![](http://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=xshubhamg&theme=nord_bright)

`http://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username={username}&theme={theme_name}&exclude={exclude}`
- Accept url parameters
  - theme
    - Theme name
  - username
    - Username
  - exclude:
    - A comma separated list of languages to exclude, e.g., exclude=java,rust,jupyter%20Notebook
      - You can represent a space in the language list by using '%20' when you want to include a space.
    - You can found the supported languages in [here](https://github.com/github/linguist/blob/master/lib/linguist/languages.yml)

### GitHub stats card
![](http://github-profile-summary-cards.vercel.app/api/cards/stats?username=xshubhamg&theme=nord_bright&)

`http://github-profile-summary-cards.vercel.app/api/cards/stats?username={username}&theme={theme_name}`
- Accept url parameters
  - theme
    - Theme name
  - username
    - Username

### Productive time card
![](http://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=xshubhamg&theme=nord_bright&utcOffset=8)

`http://github-profile-summary-cards.vercel.app/api/cards/productive-time?username={username}&theme={theme_name}&utcOffset={utcOffset}`
- accept url parameters
  - theme
  - username
  - utcOffset

---

## How to use (GitHub Actions)

This action generate your github profile summary cards and make a commit to your repo.
You can also trigger action by yourself after add this action.

:star: [Follow tutorial](https://github.com/xshubhamg/github-profile-summary-cards/wiki/Tutorial) ( Recommendation ) :star:

#### First step

- You need create a [Personal access token](https://docs.github.com/en/github/authenticating-to-github/creating-a-personal-access-token) with correct permissions.
  [Personal token](https://github.com/xshubhamg/github-profile-summary-cards/wiki/Tutorial#generate-token)

- Add personal access token to repo secret.

#### Use template ( create a repository )

- [github-profile-summary-cards-example](https://github.com/xshubhamg/github-profile-summary-cards-example)

- Action already setup in this template, you just need click `use this template button` to create your profile readme.

- After replace GITHUB_TOKEN with your repo secret and trigger action you can use everything in `profile-summary-card-output` folder.

#### Add to exist repository

- Add this action to repo and replace GITHUB_TOKEN in action yml file with your repo secret.

---

## GitHub Actions usage

After the action finished. You can see all of summary cards are in folder which named `profile-summary-card-output`.

`Note: Some summary cards might not be updated in time, because github raw file has cache time.`

```yml
name: GitHub-Profile-Summary-Cards

on:
  schedule: # execute every 24 hours
    - cron: "* */24 * * *"
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest
    name: generate-github-profile-summary-cards
    permissions:
      contents: write

    steps:
      - uses: actions/checkout@v4
      - uses: xshubhamg/github-profile-summary-cards@release
        env: # default use ${{ secrets.SUMMARY_GITHUB_TOKEN }}, you should replace with your personal access token
          GITHUB_TOKEN: ${{ secrets.SUMMARY_GITHUB_TOKEN }}
        with:
          USERNAME: ${{ github.repository_owner }}
          # BRANCH_NAME is optional, default to main, branch name to push cards
          BRANCH_NAME: "main"
          # UTC_OFFSET is optional, default to zero
          UTC_OFFSET: 8
          # EXCLUDE is an optional comma seperated list of languages to exclude, defaults to ""
          EXCLUDE: ""
          # AUTO_PUSH is optional, a boolean variable default to true, whether automatically push generated files to desired branch
          AUTO_PUSH: true
```

---

## Development (Devbox)

This project uses [devbox](https://www.jetify.com/devbox) to ensure a reproducible development environment (Node.js 22, Python 3).

### 1. Setup
```sh
# Install devbox
curl -fsSL https://get.jetpack.io/devbox | bash

# Enter shell (installs all dependencies automatically)
devbox shell
```

### 2. Local Testing
We provide a script to generate cards locally for visual verification.
**Prerequisite**: You must have a `GITHUB_TOKEN`.

```sh
# Set token (or add to .env)
export GITHUB_TOKEN=your_token_here

# Run local test generator
npm run test:local
```
Outputs will be saved to `debug_output/` folder.

### 3. Run Vercel API Locally
```sh
npm i -g vercel
vercel dev
```

## Deployment

For detailed instructions on how to deploy your own instance of GitHub Profile Summary Cards (e.g., to Vercel), please refer to our [Deployment Guide](deployment.md).

