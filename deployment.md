# Deployment Guide (Vercel)

This guide provides instructions for deploying your own instance of GitHub Profile Summary Cards to Vercel.

## Prerequisites

1.  **GitHub Account**: You need a GitHub account to fork the repository.
2.  **Vercel Account**: Sign up at [vercel.com](https://vercel.com).
3.  **Personal Access Token (PAT)**:
    *   Go to [GitHub Settings > Developer settings > Personal access tokens > Tokens (classic)](https://github.com/settings/tokens).
    *   Generate a new token with `repo` and `user` scopes.
    *   **Keep this token safe!** You will need it for the `GITHUB_TOKEN` environment variable.

## Deployment Steps

### Option 1: Deploy with Vercel Button (Recommended)

Click the button below to fork the repo and deploy it to Vercel instantly:

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fvn7n24fzkq%2Fgithub-profile-summary-cards&env=GITHUB_TOKEN&envDescription=https%3A%2F%2Fgithub.com%2Fvn7n24fzkq%2Fgithub-profile-summary-cards%23first-step&project-name=my-github-profile-summary-cards)

During the setup, Vercel will ask you to provide the `GITHUB_TOKEN`. Paste your Personal Access Token there.

### Option 2: Manual Deployment via Vercel Dashboard

1.  **Fork the Repository**: Fork [vn7n24fzkq/github-profile-summary-cards](https://github.com/vn7n24fzkq/github-profile-summary-cards) to your own GitHub account.
2.  **Import to Vercel**:
    *   On the Vercel dashboard, click **Add New > Project**.
    *   Import your forked repository.
3.  **Configure Environment Variables**:
    *   In the "Environment Variables" section, add:
        *   **Key**: `GITHUB_TOKEN`
        *   **Value**: Your GitHub Personal Access Token.
4.  **Deploy**: Click **Deploy**. Vercel will automatically detect the configuration and build the project.

### Option 3: Local Deployment via Vercel CLI

1.  Install the Vercel CLI: `npm i -g vercel`
2.  Login: `vercel login`
3.  Run `vercel` in the project root and follow the prompts.
4.  Add the secret: `vercel env add GITHUB_TOKEN` (then paste your token).
5.  Deploy to production: `vercel --prod`

## Configuration & Customization

### Environment Variables

| Variable | Description | Required |
| :--- | :--- | :--- |
| `GITHUB_TOKEN` | Your GitHub Personal Access Token. Used to fetch data from the GitHub API. | **Yes** |

### Custom Domains

You can add a custom domain to your Vercel project under **Project Settings > Domains**.

## Maintenance

To keep your instance up to date with the original repository:
1.  Go to your forked repository on GitHub.
2.  Click **Sync fork > Update branch**.
3.  Vercel will automatically trigger a new deployment for the updated code.

## Troubleshooting

- **Rate Limiting**: If you see empty cards or errors, ensure your `GITHUB_TOKEN` is valid and has not exceeded its rate limit.
- **Build Failures**: Check the "Deployments" tab in the Vercel dashboard for detailed build logs.
