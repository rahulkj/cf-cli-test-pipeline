Sample pipeline to generate report using cf cli & send emails
---

## How to Use?

Simple, begin with updating the [params.yml](./params.yml) and entering the environment specific details. This pipeline will use your `pivnet_token` to pull down the `platform-automation-image` and `cf cli`.

## Test the pipeline

Just fly the pipeline usng the `fly` cli

```
fly -t some-team sp -p cf-test -c cf-pipeline.yml -l params.yml
```

Trigger the pipeline from the UI/CLI.

## Email output would look like this:

```
Build finished: cf-test/simple-report/1

Getting orgs as admin...

name
p-spring-cloud-services
system
```

Go ahead and get creative to send some awesome reports!!