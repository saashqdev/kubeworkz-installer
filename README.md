# Kubeworkz-Installer

Kubeworkz installer installs Kubeworkz by the "all-in-one" method. More details follow [doc](https://kubeworkz.io/docs/installation-guide/).

## Quick start

Set version

```bash
export KUBEWORKZ_VERSION=v1.8
```

### All in one install

```bash
curl -fsSL https://kubeworkz.s3.amazonaws.com/kubeworkz-installer/release/v1.3/entry.sh | bash
```

### Custom install

```bash
export CUSTOMIZE="true";curl -fsSL https://kubeworkz.s3.amazonaws.com/kubeworkz-installer/release/v1.3/entry.sh | bash
```

## Clean UP

```bash
curl -o cleanup.sh https://kubeworkz.s3.amazonaws.com/hack/cleanup.sh
```

```bash
# params can be: 'kubeworkz','k8s','docker','containerd','all'
/bin/bash cleanup.sh all
```
