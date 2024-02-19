# Requirements

For cilium pods to work, the owner of the /opt/cni/bin directory must be `root`

1. If you have already done cluster up through kubespray, do it manually on each node!
```
chown root:root /opt/cni/bin
```
2. If you haven't set up a cluster yet, just change some configurations before running kubespray

`kubespray/roles/network_plugin/cni/tasks/main.yml` 

In default!

![image](https://github.com/bexruzdiv/cilium/assets/107495220/4dd0bf98-8c24-4864-adcf-b449d43f7cc7)


You need to change!
Just change owner to `root`

![image](https://github.com/bexruzdiv/cilium/assets/107495220/77cdcb50-8a05-4b7f-9ae2-9de5d16a0c66)
