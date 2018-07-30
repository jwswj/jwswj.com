# jwswj.com

Public website.

Infrastructure maintained by Terraform in [https://github.com/jwswj/jwswj.com-ifra](https://github.com/jwswj/jwswj.com-ifra)

## Development

```
bin/dev
```

## Deployment

Deployment is managed by AWS CodePipeline and CodeBuild. A commit to master
automatically triggers the CodePipeline, during the build it completes a COPY
of the files in the `public` folder to the production S3 bucket.
