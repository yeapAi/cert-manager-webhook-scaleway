## Helm release

In the branch gh-pages which is used by github for github pages create an empty file index.yaml

Generate the release with the command:

```ssh
cd deploy
helm package scaleway-webhook
```

Move the tgz file at the root of the repository

Update index file with

```ssh
helm repo index . --url https://yeapai.github.io/cert-manager-webhook-scaleway/
```

Commit all change in gh-pages branch.
