# kubernetes-ambassador-lyft-ratelimit
Helm charts to deploy lyft's ratelimit (https://github.com/lyft/ratelimit) to kubernetes

Steps: 
1. Follow Ambassador Documentation to setup: https://www.getambassador.io/user-guide/getting-started
2. Deploy lyft-ratelimit with included charts
3. Update the test qotm service with `qotm-rate-limited.yaml`. This will rate limit the service at 5 per minute per ip with the config. 