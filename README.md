# Docker image to use jelastic and jq  in gitlab ci

> This image is based on https://github.com/mwienk/docker-jelastic-cli

## Jelastic cli usage

In a Gitlab job

```yaml
# ...
deploy:
  image: mwienk/jelastic-cli
  script:
    - /root/jelastic/users/authentication/signin --login $LOGIN --password $PASSWORD --platformUrl $PLATFORM_URL
    - /root/jelastic/environment/control/getenvs
```
