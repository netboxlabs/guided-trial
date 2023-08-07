# Explore the device NLAMS01-SW-1 

Follow these steps to understand how NetBox models the following objects:

- Device types
- Device roles
- Platforms
- Management IPs
- Module bays
- Interfaces
- Console ports
- Power ports
- Cables


## Steps:

1. From within the Amsterdam rack (`Organisation` > `Racks` > `NLAMS01-RK-01`) click on the device called `NLAMS01-SW-1`
2. In the Device panel, note the `Device Type` is a `Juniper EX4300-48P`.
3. In the Management panel note the Status is `Active`, the device role is `Access Switch`. Also note the `Platform` type and the `Primary IPv4` address`.
4. Along the top menu, click on `Interfaces`, then click in interface `ge-0/0/1`. Note the interface type, and the 802.1Q mode. 
5. In the `Related Interfaces` panel, note this is a member of a `LAG`(Aggregated Interface) called `ae0`. 
6. In the `Connection` panel on the right hand side note that this interface is directly connected to device `NLAMS01-VSP-1` port `Gig-E 1` . Click on the Trace icon next to `Cable` to view the trace. Note the cable type, color and length. 
7. Go back to the device and click on `Console Ports`, note the cable connected to the Console server port. 
8. Go back to the device and click `Power Ports` and note that both ports are connected to separate PDUs and outlets. 
