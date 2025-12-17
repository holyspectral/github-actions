# Container build

This action builds, pushs, and signs container images based on input.

## Inputs

| Parameters | Description                                                                                     | Default    | Required |
| ---------- | ----------------------------------------------------------------------------------------------- | ---------- | -------- |
| arch       | List of target architectures to build.                                                          | amd64      | true     |
| dockerfile | The relative path of dockerfile that this action will build                                     | Dockerfile | true     |
| repo       | The repository component in a fully qualified image. For instance, ghcr.io/<repo>/<image>:<tag> | n/a        | true     |
| image      | The target image name in a fully qualified image.                                               | n/a        | true     |
| tag        | The tag component in a fully qualified image.                                                   | n/a        | true     |
| GH_TOKEN   | The GitHub token with the permission to publish images to ghcr.                                 | n/a        | true     |