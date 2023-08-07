# Explore the Amsterdam Site

Follow these steps to understand: 
- Sites
- Topologies (via a plugin)
- Racks
- Devices
- Wireless LANs
- Circuits
- Power Panels and Feeds

## Steps:
1. Click Organization, Sites, Amsterdam
2. Note the Region is Netherlands, within the Europe parent region
3. Note that site is a member of the Branch group, and has a status of Active
4. Note that Tenant associated with the site is called Consulting, which is part of the Divisions Tenant Group
5. Note the other fields containing information about the locale and time zone
6. Explore the Related Objects panel on the right to see what objects are associated with the Amsterdam site, such as Locations, Racks, Devices, and Circuits
7. Note that there is an Operations contact (Eric) associated with the site
8. Scroll down to locations and note that there is one location called Comms Room and it contains a single rack with 10 Devices in it. 
9. Scroll further down and notice the 2 un-racked devices, which are Wireless Access Points  
10. Click on the Topology icon (top right of the screen) to explore how the devices are connected. Zoom in and out and drag devices around. Note that this Topology Viewer is a plugin, and that many other plugins are available to easily extend NetBox core functionality
11. Within Related Objects, click the ‘1’ next to Racks and then click in the name of the rack `NLAMS01-RK-01`
12. In the Rack panel note the Role of the rack is Infrastructure, and that you can define these roles to suit your requirements. Also note the Space and Power Utilization
13. In the Dimensions panel, note the type of panel is a 4 post cabinet, 19 inches in width, with 42 rack units of space, and that you can define other types of racks. 
14. Explore the Front and rear rack elevations. 
15. In the main menu on the left hand side, select Wireless > Wireless LAN Groups, Then select Europe_WLANS. 
16. In the Related Objects panel, click on Wireless LANs, then select on of the SSID’d to examine it’s properties
17. In the main menu on the left hand side, select Circuits > Providers and click on the provider KPN. Examine the properties of the provider
18. Scroll down to the Circuits panel and click on the circuit ID KPNCir1234, and examine the properties of the circuit
19. In the Termination Z panel on the right hand side, click the Trace icon to trace the cable, and note the device and interface that the cable terminates on
20. In the main menu on the left hand side, click Power > Power Panels and then click on panel NLAMS01-PWR-PAN-1
21. Scroll down to Power Feeds, and click on the feed NLAMS01-PWR-FEED-1. Examine the properties and electrical characteristics. 
22. In the Connection panel on the right hand side, click note the Path Endpoints and click on the NLAMS01-PDU-1 PDU. Explore the Device, Management and Power Utilization information.
23. On the Power Outlets tab at the top, note the cables connecting devices to the PDU