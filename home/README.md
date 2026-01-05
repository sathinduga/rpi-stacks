```
mkdir -p /home/sathindu/HomeLab/volume-mounts/home-homeassistant/config
mkdir -p /home/sathindu/HomeLab/volume-mounts/home-matterserver/data
```

```
infisical export --env=prod --path=/stacks/home/homeassistant --format=dotenv > /home/sathindu/HomeLab/infisical-secrets/.infisical.stacks.home.homeassistant.env
```