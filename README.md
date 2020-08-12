# sealed-secrets-kubeseal-nsg

[![Get it from the Snap Store](https://snapcraft.io/static/images/badges/en/snap-store-black.svg)](https://snapcraft.io/sealed-secrets-kubeseal-nsg)

Kubeseal is the client for Sealed Secrets for Kubernetes.

The kubeseal utility uses asymmetric crypto to encrypt secrets that only the cluster can decrypt.
These encrypted secrets are encoded in a SealedSecret resource, once unsealed this will produce a normal
Secret inside the cluster.

For more information see https://github.com/bitnami-labs/sealed-secrets

There are a few limitations due snapd's sandbox:

* You can only read files from your home directory.
* You can't read from hidden files (starting with a dot)
* On Ubuntu Core you need to manually connect the home interface

## Install

```
snap install sealed-secrets-kubeseal-nsg
```

If you like to use the shorter command "kubeseal" add an alias:

```
sudo snap alias sealed-secrets-kubeseal-nsg kubeseal
```
