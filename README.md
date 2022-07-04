# Role: awx

Configure awx on a Kubernetes cluster. For the moment, this assumes a K3S cluster on the targeted node.

## Configuration
| Variable             | Default vaule                    | Description                                    |
|----------------------|----------------------------------|------------------------------------------------|
| `awx_version`        | `0.23.0`                         | AWX version to install                         |
| `awx_port`           | `31852`                          | Port to expose AWX on                          |
| `awx_redis_version`  | `bullseye`                       | version of redis to use for the embedded redis |
| `awx_ee`             | `quay.io/ansible/awx-ee:latest`  | AWX execution environment to use               |

This role is fairly basic at this point: It'll setup the officially supported awx operator in a local k3s cluster.

**Compatibility tested with:**
  * Debian 11 + our K3S role

## License
GPLv3
