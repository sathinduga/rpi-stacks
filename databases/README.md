# Databases Stack

## Required Secrets in Infisical

Path: `/stacks/databases/postgres`

```
POSTGRES_PASSWORD
HA_USER_PASSWORD
N8N_USER_PASSWORD
```

## Pull Secrets

```bash
infisical export --env=prod --path=/stacks/databases/postgres --format=dotenv > /home/sathindu/HomeLab/infisical-secrets/.infisical.stacks.databases.postgres.env
```
