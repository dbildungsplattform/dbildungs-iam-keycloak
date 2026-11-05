Installing Custom Providers
===========================

Files in this directory are used to add custom provider JAR files to Keycloak.

Adding new providers to this directory will take effect only after a new build.

SPSH Protocol Mappers
--------------------

The SPSH OIDC and SAML mappers are supplied by [keycloak-providers-1.8.jar](keycloak-providers-1.8.jar).
Do not install legacy SPSH mapper JARs alongside it: different builds of the same
`com.spsh` classes and protocol mapper registrations must not be present in the image.

When replacing a provider, remove any superseded JAR before rebuilding the image.

