# GitHub Action to Download Files from S3 Bucket

### Usage example

```
- name: Download master bundle stats from S3
  uses: fxtr/ga-s3-download@master
  env:
    AWS_ACCESS_KEY_ID: ${{ secrets.AWS_ACCESS_KEY_ID }}
    AWS_SECRET_ACCESS_KEY: ${{ secrets.AWS_SECRET_ACCESS_KEY }}
    AWS_REGION: eu-west-1
    AWS_S3_BUCKET: fixter-travis-artifacts/bundles/master.json
    DEST_DIR: ./bundles
    RECURSIVE: true
```