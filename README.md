# Charts
The AD's helm charts repository

## usage

### Add Repo
```bash
$ helm repo add ad-stable https://pnet.github.io/charts/
$ helm repo update
```

### Install

```bash
$ helm upgrade release_name ./deploy/helm/chart-ad/ \
    --install \
    --wait \
    --timeout=300s \
    --values=path/to/custom_values.yaml \
    --values=path/to/custom_values2.yaml \
    --set foo.bar=value \
```

### Custom values

You can supply as many custom values files as you want using `--values` or `-f` flag.
[here](https://github.com/PNet/charts/blob/main/stable/chart-ad/values.yaml) you can find a custom
values file example.