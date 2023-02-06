# NVIDIA Cumulus Linux Virtual Workshop (aka Test Drive) Automation

This repository holds automation scripts for the NVIDIA Cumulus Linux Virtual Workshop (aka Test Drive) Lab. 

This repository is cloned by the `oob-mgmt-server-customizations.sh` script (located in the repository [here](https://gitlab.com/lsimpson762/virt-workshop-snapshot-creation)) in order to create the `Test-Drive-Automation` directory on the `oob-mgmt-server`. This is done during the CI/CD workflow to create the base snapshot and cloned simulation for testing purposes.

The attendees of the event use this automation during two steps that are documented in the lab guide. 

The first step in the lab guide is to run the ansible playbook `start-lab.yml` to set up the base configuration for the servers in the lab. The `lab3.yml` is run at the completetion of Lab 2 in order to provide a configuration that removes the interswitch links from leaf01-leaf02 so that BGP routing through the spine01 switch can be configured and tested.

The lab guide is available upon request and is provided to the attendees of the event through the marketing channel.
