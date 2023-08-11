# Sentinel policy examples

Lab files used by the [Sentinel policy examples](https://developer.hashicorp.com/vault/tutorials/policies/sentinel-validation-policies) tutorial.

Example Sentinel policies that illustrate how Sentinel can be used in Vault
Enterprise to validate that specific keys of secrets adhere to certain formats.
It includes policies that validate zip codes, state codes, AWS keys, and Azure
credentials. It also includes a policy that requires the `delete_version_after`
metadata property of KV v2 secrets to be less than 30 days (720 hours). This
restricts the duration of versions of secrets; after this amount of time, each
version is deleted. In addition to providing 5 Sentinel policies along with
corresponding test cases for use with the [Sentinel
Simulator](https://docs.hashicorp.com/sentinel/intro/getting-started/install),
the guide shows the reader how to deploy them to a Vault server and how to test
them with the Vault CLI. The policies support both versions 1 and 2 of the [KV
secrets engine](https://developer.hashicorp.com/vault/docs/secrets/kv).


