## Postgres Chart

An example chart for deploying a postgres database on Openshift



Creating new release

```
git checkout release
helm package .
mv  postgres*.tgz release/
helm repo index --url https://jland-redhat.github.io/postgres-helm-chart/ .
git add --all
git commit -m "Updating to version x.x.x"
```


## Testing chart

### Add helm repo
```
helm repo add oauth https://jaland.github.io/oauth-helm-chart/
helm repo list
```

### Deploy chart
```
helm install oauth/oauth-chart --name-template oauth
```
