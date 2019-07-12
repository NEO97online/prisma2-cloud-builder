# Prisma2 Builder for Google Cloud Build

## Building this builder
To build this builder, run the following command in this directory.
```
$ gcloud builds submit
```

The builder will then be available at `gcr.io/$PROJECT_ID/prisma2`.

## Usage

Add this step to your `cloudbuild.yaml`:
```yaml
steps:
  - name: 'gcr.io/$PROJECT_ID/prisma2'
    args: ['generate']
```
