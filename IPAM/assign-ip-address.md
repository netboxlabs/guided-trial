# Assign an IP address to the Amsterdam router

Follow these steps to assign an IP address from the ISP provided prefix `37.251.64.0/29`to the external facing interface `GigabitEthernet0/0/1` of the WAN Router `NLAMS01-RTR-1` in Amsterdam

1. In the left hand main menu, click on **IPAM** and **Prefixes** and click on the **ISP Assigned** prefix `37.251.64.0/29`. 
2. Click on the **IP Addresses** tab, and note that `.1` is already assigned to the ISP Router. Then click **Add IP Address**. Note that the next available IP address `.2` has been pre-populated. 
3. Scroll down to **Interface Assignment**, leave **Device** highlighted and click on the **Selector** button on the right hand side.
4. In the left hand panel click **Device** and then click on the **+** on the right hand side to select the device
5. Scroll down and select `NLAMS01-RTR-1` and then click search, then select `GigabitEthernet0/0/1`
6. Click **Create**
7. To Verify the assignment, navigate to **Devices** > **NLAMS01-RTR-1** > **Interfaces** > **GigabitEthernet0/0/1** and scroll down to the **IP Addresses** panel. 