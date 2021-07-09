# Flyyer Actions and Workflows for GitHub

![deploy results](./assets/result.png)

## Create workflow file

Create the following file in your repository:

```sh
mkdir -p .github/workflows
touch .github/workflows/deploy.yml
```

Copy the contents of from [workflow-templates/flyyer-yarn.yml](./workflow-templates/flyyer-yarn.yml) to your `.github/workflows/deploy.yml`.

### Via `curl`:

Write these two lines on your terminal:

```sh
mkdir -p .github/workflows
curl -L https://raw.githubusercontent.com/useflyyer/flyyer-actions/main/workflow-templates/flyyer-yarn.yml --output .github/workflows/deploy.yml
```

## Add `FLYYER_KEY` to your Github's secrets

Get your `FLYYER_KEY` from [https://flyyer.io/settings/keys](https://flyyer.io/settings/keys) then add it to your **Settings -> Secrets** inside the settings of your repository.

![secrets section in your repository's settings](./assets/settings-secrets.png)

## Help needed

- Convert to an actual Github Action.
- Create NPM alternative and make it easy to switch between Yarn and NPM.
