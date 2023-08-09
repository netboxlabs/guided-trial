# Import IPAM Data for the Los Angeles Site

Follow these steps to manually create a VLAN Group and then bulk import VLANs and Prefixes from spreadsheet data (.csv) files. 

Before starting this exercise, download the 2 files you will need be importing: 

[VLAN Data](https://github.com/netboxlabs/guided-trial/blob/develop/LA_VLANs.csv)
[Prefix Data](https://github.com/netboxlabs/guided-trial/blob/develop/LA_prefixes.csv)

These are CSV files containing the new VLAN and Prefix data to be bulk imported. Inspect the files to understand the data being imported.

1. In left-hand main menu click on **IPAM** > **VLAN Groups**, and note the existing VLAN Group for Amsterdam `NLAMS01_VLANS`.
2. Click **Add** and name the new group `USLAX01_VLANS`, add `Los Angeles VLANs` as the description. 
3. Set the **scope** to `DCIM > Site`, the **Region** to `California`, **Site Group** to `Branch` and the **Site** to `Los Angeles`, then click **Create**
4. In left-hand main menu under **IPAM** > **VLANs**, click the blue **up arrow** symbol to import data, and click on the **Upload File** tab underneath **VLAN Bulk Import** 
5. Click on **Choose file** and then browse then select the file `LA_VLANs.csv` from your downloads directory, and click **Submit** to import the VLANs. Note VLANS are all members of the `USLAX01_VLANs` group and are scoped to the `Los Angeles` site. 
6. In left-hand main menu under **IPAM** > **Prefixes**, click the blue **up arrow** symbol to import data, and click on the **Upload File** tab underneath **Prefix Bulk Import** 
7. Click on **Choose file** and then browse then select the file `LA_prefixes.csv` from your downloads directory, and click **Submit** to import the Prefixes. Note the `192.168.4.0/22` Supernet has 6 child prefixes.  
8. To verify the new new data, navigate to **Organization** > **Sites** > **Los Angeles** and from the **Related Objects** panel explore the new `Prefixes`, `VLAN Group` and `VLANs` you just created. 

For a next step why not try uploading some of your own IPAM data?