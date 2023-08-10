# Explore NetBox Provisioning

Follow these steps to get familiar with the following: 
- Data sources
- Config contexts
- Config templates

### Data Sources   
1. In the Web UI main menu, navigate to **Operations** and click **Data Sources**, and click on the data source called `Guided Trial Data Source`
2. Note the Data Source properties - this is a remote Git repository and it has been set to ignore any `.md` or `.csv` files. Data Sources can be either the local file system, a remote Git repo or an Amazon S3 Bucket. 
3. scroll down to the **Files** section and click on the file called `	cisco-switch-template-example.j2` This is a Jinja 2 template file for a Cisco Switch that is being used to render the full configuration for Cisco 9200-24P device types.   
4. Click the back button in your browser and in the **Files** section, click on the file called `sydney-config-context.json` this contains data in `JSON` format that is used in a **Config Context** for devices in the `Sydney` site. 
5. Try adding a new **Data Source** by navigating to **Operations** and click **Data Sources** again. In the top-right corner click on **+ Add**, give it a name and choose either `Git` or `Amazon S3` for the **Type**. Fill out the rest of the form and click **Create**

### Config Contexts
1. In the Web UI main menu, navigate to **Provisioning** > **Config Contexts** and click on the one called `Sydney Network Services`.
2. Note the **Data Source** and **Data File**, and that the **Assignment** is at the `Sites` level and specifically the `Sydney` site. This means that this Config Context will apply to any devices in the `Sydney` site. 
3. Note the **Data** on the right-hand side. This data will be pulled into the **Config Template** along with the device data from NetBox to render the full device configuration in later steps. 

### Config Templates
1. In the Web UI main menu, navigate to **Provisioning** > **Config Templates** and click on the one called `Cisco Switch - Basic`.
2. Note the **Data Source** and **Data File**, and that the content of the **Template** itself.
3. Device data from NetBox and the **Config Context** data will be pulled in render the full device configuration in later steps. 

### Render the Device Configuration in the UI
1. This **Config Template** will be used by the switch `AUSYD01-SW-1`. To see where this is assigned, navigate to **Devices** > **AUSYD01-SW-1**, then click on **Edit** in the top-right corner. 
2. Under **management** note the **Config Template** is `Cisco Switch - Basic`. 
3. Click **Cancel** and then along the top tabs click on **Config Context** and note the **Rendered Context**
4. Click on **Render Config** to view the complete device configuration, then click on **Download** on the right hand side to download as a text file.