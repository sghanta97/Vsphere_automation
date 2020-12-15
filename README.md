# Vsphere_automation
Automate VM creation along with the required network topology on Vmware ESXI


## network_infrastructure_create.py
User will give input in CSV table ( rows are port grps , columns are VMs ).  
In the table: 
* 0 -> no interface is attached to this port grp
* <custom> -> you can give your custom IP address ( usually if it is Public Ip )
  
If the port grps are already not present then the port groups and switches are created.
The Entire topology created is stored in a "Topology" file and is also printed out on the console. 


** how to handle the image ( use scp/ftp to download the image and use it from there on )

Note:
* The Vms hostname should be unique
* while assigning IP address make sure they are unique in that network 


