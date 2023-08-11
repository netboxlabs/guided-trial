# Add a New Device to the Rack

Get hands on with NetBox by adding a new switch to the rack in Amsterdam (`NLAMS-RK-01`). Follow these steps to understand how to:

- Add new devices directly into the desired rack unit
- Define the device properties like Device Type, Platform etc
- Connect Power, Console and Network cables
- View the amended network Topology (via a plugin)


## Steps 
1. From the Amsterdam rack (**Organisations** > **Racks** > **NLAMS01-RK-01**) hover your mouse over rack unit `38`, which is underneath device `NLAMS01-SW-1`, and click **add device**.
2. Name the device `NLAMS01-SW-2`.
3. Select `Access Switch` from the drop-down menu for the **Device role**.
4. For **Device Type**, select `EX4300-48P`.
5. For **Airflow** select `Front to rear`.
6. Under **Management** - **Platform** select `Juniper JunOS`.
7. Under **Tenancy** select `Divisions` for the **Tenant group**, and `Consulting` for the **Tenant**.
8. Click **Create**.
9. From the top menu click on **Power Ports**, select `PSU0` and click the green **add cable** icon and select `Power Outlet`. For the B side select device `NLAMS01-PDU-1` and `Power Outlet 5`, select `Power` for the `type`, and click **create**.
10. Select `PSU1` and click the green **add cable** icon and select `Power Outlet`. For the B side select device `NLAMS01-PDU-2` and `Power Outlet 5`, select `Power` for the cable **type**, and click create.
11. Click on **Console Ports**, select `Console RJ45` and click the green **add cable** icon and select `Console Server Port`. For the B Side select `NLAMS01-CON-1` port `ttys3`, and `CAT6` as the cable **type**, and click **Create**.
12. Click on the **Interfaces** tab, select interface `et-0/1/0` and click the green **add cable** icon and select `Interface`. For the B-Side, select device `NLAMS01-SW-1` interface `et-0/1/0`, and `Direct Attach Copper (Passive)` as the **Type**, **Color** `Black` and **length** `2 Meters`, and click **Create**
13. Repeat this for interface `et-0/1/1` (note that it is possible to upload objects like cables in bulk from CSV, JSON and YAML data and files) 
14. From the interfaces list select both interfaces `et-0/1/0` and `et-0/1/1` and click **Edit** (bottom left).
15. Scroll down to **802.1Q Switching** and set the **Mode** to `Tagged All`, and the **VLAN Group** to `NLAMS01_VLANS`, and click **Apply**.
16. Repeat steps 14 and 15 for the same two interfaces on switch `NLAMS01-SW-1`
17. Navigate back to the Amsterdam site (**Organisations** > **Sites** > **Amsterdam**) and click on the **Topology** icon to view the new topology now that you have added a 2nd switch to the rack. 