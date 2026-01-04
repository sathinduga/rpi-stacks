# Grafana Alloy Secrets

## Required Secrets in Infisical

Path: `/stack/grafana`

`GRAFANA_CLOUD_LOKI_URL`
`GRAFANA_CLOUD_LOKI_USERNAME`
`GRAFANA_CLOUD_PROMETHEUS_URL`
`GRAFANA_CLOUD_PROMETHEUS_USERNAME`
`GRAFANA_CLOUD_TEMPO_URL`
`GRAFANA_CLOUD_TEMPO_USERNAME`
`GRAFANA_CLOUD_API_KEY`

## Getting Credentials from Grafana Cloud

1. Go to [grafana.com](https://grafana.com) → Your Stack
2. **Loki (Logs):** Connections → Hosted Logs → Details
3. **Prometheus (Metrics):** Connections → Hosted Prometheus → Details
4. **Tempo (Traces):** Connections → Hosted Traces → Details
5. **API Key:** Security → Access Policies → Create token with `metrics:write`, `logs:write`, `traces:write`

## Pull Secrets
```bash
infisical export --env=prod --path=/stacks/grafana --format=dotenv > /home/sathindu/HomeLab/infisical-secrets/.infisical.stacks.grafana.env
```

## Verify
```bash
cat /home/sathindu/HomeLab/infisical-secrets/.infisical.stacks.grafana.env
```