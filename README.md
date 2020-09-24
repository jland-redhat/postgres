## Postgres Chart

An example chart for deploying a postgres database on Openshift



Creating new release

```
git checkout release
helm package .
mv  postgres-chart*.tgz release/
checkout release
git repo index --url https://jland-redhat.github.io/postgres-helm-chart/
```
