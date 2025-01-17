+++
title = "Docker Compose"
weight = 30
+++

Docker Compose mode deploy a full environnement with a pre-configured Prometheus and Grafana.

## Requirements
* Windows, Linux or macOS 
* Docker (> 19.03)
* Docker-Compose

## Steps

1. Download the source code of the project from the [latest release](https://github.com/pbrissaud/suivi-bourse/releases/latest) and extract it.

2. Move to the downloaded folder and go to **docker-compose** folder

3. Edit `config.yaml`file following the [chapter 3](/config)

4. To start the stack, execute this command in your shell: 
```Bash
docker-compose up -d
```

## Environment variables

Env variables can be used to override some default parameters : 

| ENV                  | Description                                                     | Default Value |
|----------------------|-----------------------------------------------------------------|---------------|
| SB_SCRAPING_INTERVAL | Interval in seconds where app gets data from Yahoo! Finance API | 120           |

Edit **.env** file in the **docker-compose** folder to set environment variables.