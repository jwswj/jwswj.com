# jwswj.com

A very static website running at https://jwswj.com.

Infrastructure maintained by Terraform in [https://github.com/jwswj/jwswj.com-infra](https://github.com/jwswj/jwswj.com-infra)

## Development

```
bin/dev
```

## Deployment

Deployment is managed by AWS CodePipeline and CodeBuild. A commit to master
automatically triggers the CodePipeline, during the build it completes a COPY
of the files in the `public` folder to the production S3 bucket.
