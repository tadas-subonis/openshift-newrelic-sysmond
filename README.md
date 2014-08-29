openshift-newrelic-sysmond
==================

NewRelic plugin for OpenShift Deployments. It is supposed to monitor health per-Gear
basis by utilising the newrelic-sysmond app. The results should appear in your "Server" section.

Install
-------

- Install the cartridge from GitHub.

```
  rhc cartridge add  https://raw.githubusercontent.com/tadas-subonis/openshift-newrelic-sysmond/master/metadata/manifest.yml \
	-a <your_app_name> \ 
    -e OPENSHIFT_NEWRELIC_LICENSE_KEY=<your_new_relic_key>
```

- Restart your application.

```
  rhc app restart <your_app_name>
```
      
Remove
------

```
  rhc cartridge remove newrelic-sysmond -a <your_app_name>
```
