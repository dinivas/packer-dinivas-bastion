# Packer Dinivas proxy image

This __packer__ project build Dinivas proxy image

```sh
# For Openstack
packer build -only=openstack -var 'ssh_user=XXXX' -var 'source_image_id=XXXXXXX' -var 'flavor=XXXXXX' template.json

# For DigitalOcean
packer build -only=digitalocean  -var 'region=fra1' -var 'ssh_user=root' -var 'source_image_name=87674237' -var 'flavor=s-1vcpu-2gb-intel' template.json
```

## Environement variables

### OPENSTACK

### DIGITALOCEAN

The following env variables can be set:

```
export DIGITALOCEAN_API_TOKEN=XXXXX
```