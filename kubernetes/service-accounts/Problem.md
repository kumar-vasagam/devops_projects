Problem # 1 we are trying to solve:

1. Create one Job on `maintenance` namespace
2. Create one busybox pod on `dev` namespace.
3. Create the infrastructure that enables busybox pod to "see the Job" pod. (don't know what they mean by "see" - from: https://kubernetes.io/docs/concepts/security/service-accounts/#cross-namespace)

Problem #2:
There is a Prod server and a Test server both need a secret. Instead of creating 2 separate pod definition files, create 2 separate service accounts and simplify the pod definition (as mentioned in [here](https://kubernetes.io/docs/tasks/inject-data-application/distribute-credentials-secure/#provide-prod-test-creds))