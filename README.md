# test
replace >> token <<

## how to run this as an accelerator
Apply the following
```yaml
apiVersion: accelerator.tanzu.vmware.com/v1alpha1
kind: Accelerator
metadata:
  name: test-multival-options
spec:
  tags:
    - draft
    - test-multival-options
  git:
    url: https://github.com/jldec/test-multival-options
    ref:
      branch: main
```

## how to run this locally
- clone this repo
- edit POST.json to point to this directory on your filesystem
- start the engine (default port 8080)
- `curl http://localhost:8080/invocations -d @POST.json -H "Content-Type: application/json"`
