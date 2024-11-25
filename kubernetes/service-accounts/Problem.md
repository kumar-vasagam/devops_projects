Problem we are trying to solve:

1. Create one Job on `maintenance` namespace
2. Create one busybox pod on `dev` namespace.
3. Create the infrastructure that enables busybox pod to "see the Job" pod. (don't know what they mean by "see" - from: https://kubernetes.io/docs/concepts/security/service-accounts/#cross-namespace)