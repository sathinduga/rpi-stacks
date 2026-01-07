# Home Stack

## Create Directories

```bash
mkdir -p /home/sathindu/HomeLab/volume-mounts/home-homeassistant/config
mkdir -p /home/sathindu/HomeLab/volume-mounts/home-matterserver/data
```

## Required Secrets in Infisical

Path: `/stacks/home/homeassistant`

```
POSTGRES_DB_URL
```

## Pull Secrets

```bash
infisical export --env=prod --path=/stacks/home/homeassistant --format=dotenv > /home/sathindu/HomeLab/infisical-secrets/.infisical.stacks.home.homeassistant.env
```
