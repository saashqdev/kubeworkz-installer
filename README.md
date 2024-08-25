# Kubeworkz-Installer

Kubeworkz installer installs Kubeworkz by the "all-in-one" method. More details follow [doc](https://kubeworkz.io/docs/installation-guide/).

## Quick start

Grab a cloud box from your favorite hyperscaler - `4 cores / 8Gb RAM / 120Gb`

Do everything as `root`

Set version

```bash
export KUBEWORKZ_VERSION=v1.8
```

Install required apps
```bash
apt install sshpass conntrack unzip socat
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
