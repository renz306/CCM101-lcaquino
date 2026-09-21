# MinIO Deployment - Technical Documentation

## MinIO Container Setup

MinIO was deployed as a Docker container to provide an S3-compatible object storage service.

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
quay.io/minio/minio server /data --console-address ":9001"
```

The command runs MinIO in the background and maps the required storage service and console ports.

## Console Access

The MinIO management interface uses port:

```text
9001
```

This port was used to access the MinIO Web Console through the browser and manage the storage environment.

## Storage Bucket

A bucket was created inside the MinIO Console:

```text
client-photos
```

The bucket serves as the storage container for the files uploaded during the laboratory activity.

## Docker Configuration

Two ports were exposed by the container:

| Port   | Function          |
| ------ | ----------------- |
| `9000` | MinIO API         |
| `9001` | MinIO Web Console |

The environment variables were also configured through the `-e` option. `MINIO_ROOT_USER` defines the administrator account, while `MINIO_ROOT_PASSWORD` provides the password required for console authentication.

## Deployment Result

The MinIO container was successfully started through Docker. The Web Console was accessible through port `9001`, and the `client-photos` bucket was created for object storage operations.
