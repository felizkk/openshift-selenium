# Openshift Selenium Demo #

Author:
- Feliz Karnadi
- Karan Nayak

This repository provides the source codes to deploy selenium-hub with browser nodes.
It also provides pipeline configuration to execute selenium workloads.

Pre-requisite:
- You have a working Openfhit 4 cluster
- This has been tested with OpenShift v4.15

You will need to change all namespace details

### Dealing with API TLS Issuue ###

You can create a route, with a new host like below, and remove the tls specification.
This will accept Hub API call on non-TLS. 
**WARNING: don't do this for production.**

```yaml
http://selenium-hub-demo-selenium-nontls.apps.ocpsandbox.example.com
```
