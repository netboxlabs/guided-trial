# Explore the IPAM data for the Amsterdam site 

Follow these steps to understand how NetBox models the following object types:

- RIRs
- Aggregates
- Supernets
- Prefixes
- IP Addresses
- Prefix and VLAN roles
- VLAN groups
- VLANs


1. In the main menu on the left hand side, click on **IPAM** to expand the sub-menu options.
2. Under **AGGREGATES** click **RIRs** and note the two RIRs are **RIPE** and **RFC1918**, and also note that each one has a number of aggregates assigned to it.
3. Click on the number **3** next to **RFC 1918** to view the **Aggregates**, then click on the `192.168.0.0/16` aggregate to view the details. Note the **Family** and the **Utilization** percentage.
4. Then click on the **prefixes** tab to view the all the prefixes and their **Status**. Note that the `192.168.0.0./22` **Suspernet** has 6 **Child** prefixes. 
5. For the Child Prefixes also note the other properties, such as `VRF`, `Tenant`, `Site` and `VLAN`.
6. Click on the `192.168.2.0/26` prefix. In the **Addressing** panel on the right hand side, note the **Utilization**, and information about the IP addresses used and the **First available IP**.
7. Click on the **Addressing Details** button to display the full prefix details.
8. Click on the **IP Addresses** tab along the top to the view the assigned IP addresses. 
9. Click on `192.168.2.1/26` and note the details in the **IP Address** panel, including the **Assignment** - in this case the IP address is assigned to interface `me0` on device `NLAMS01-SW-1`.
10. In the main menu on the left hand side, click on **Prefix & VLAN Roles** to view the list of roles that have been created so far. 
11. Click on the `Branch_Data` role and in the **Related Objects** panel click on **VLANS** to see the VLANs that have this **Role** .
12. Clear the filter by either clicking on the **X** next to `Role: Branch_Data` or in the main menu on the left hand side, click on **VLANs** to display a list of all the VLANs, and note the **Group** that these VLANs are a member of. 
13. Click on the **Group** `NLAMS01_VLANS` and in the **VLAN Group** panel note the **Scope**, **Permitted VIDs**, and **Utilization**