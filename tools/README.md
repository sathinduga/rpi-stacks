# Tools Stack

## Create Directories

```bash
mkdir -p /home/sathindu/HomeLab/volume-mounts/tools-code-server/config
mkdir -p /home/sathindu/HomeLab/volume-mounts/tools-homepage/config
```

## Required Secrets in Infisical

### `/stacks/tools/code-server`

```
PASSWORD
SUDO_PASSWORD
```

### `/stacks/tools/n8n`

```
DB_POSTGRESDB_PASSWORD
N8N_RUNNERS_AUTH_TOKEN
```

### `/stacks/tools/n8n-runners`

```
N8N_RUNNERS_AUTH_TOKEN
```

## Pull Secrets

```bash
infisical export --env=prod --path=/stacks/tools/code-server --format=dotenv > /home/sathindu/HomeLab/infisical-secrets/.infisical.stacks.tools.code-server.env
infisical export --env=prod --path=/stacks/tools/n8n --format=dotenv > /home/sathindu/HomeLab/infisical-secrets/.infisical.stacks.tools.n8n.env
infisical export --env=prod --path=/stacks/tools/n8n-runners --format=dotenv > /home/sathindu/HomeLab/infisical-secrets/.infisical.stacks.tools.n8n-runners.env
```
