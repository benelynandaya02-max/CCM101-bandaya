# MinIO Deployment

## Docker Command

MinIO was deployed using Docker with ports 9000 and 9001 mapped to the container.

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=********" \
quay.io/minio/minio server /data --console-address ":9001"
```
## Web Console Port
The MinIO Web Console was accessed using port 9001.

## Bucket Name
The bucket created was client-photos.

## Environment Variables
The -e flags were used to set environment variables for the MinIO server. They defined the administrator username and password used to access the MinIO Web Console.

## Storage Operation
A sample file was uploaded to the client-photos bucket through the MinIO Web Console. This demonstrated how objects can be stored and managed using an S3-compatible object storage system.


**Important:** Keep the password as `********` in GitHub. Do **not** put the actual password in this file.

---

# 4. `reflection.md`

Create:

```text
Laboratory-05-Cloud-Data-Engineer/reflection.md
