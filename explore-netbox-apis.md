# Explore the NetBox APIs

Follow these steps to get familiar with the following: 
- REST API
- GraphQL API

## Steps:

### REST API
1. Scroll down to the footer of the Web UI. On the left hand side there are 5 icons, and a tool tip appears over each one when you hover over it. Click on the one called **REST API**. This opens a separate browser tab in the root of the REST API.
2. Explore the API from here - e.g click on the `circuits` hyperlink, and then on on `circuits` (full API request is now `GET /api/circuits/circuits/`). This API request will return all the circuits NetBox. 
3. Continue to explore the REST API and make API calls to retrieve other data from NetBox
4. Return to the main NetBox Web UI and scroll down to the footer. On the left hand side there are 5 icons, and a tool tip appears over each one when you hover over it. Click on the one called **REST API Documenation**. This opens the Swagger documentation for the REST API in a separate browser tab. 

    The Swagger docs are where you can experiment with building API calls. Note that there are sections for each areas of the NetBox data model eg. `circuits`, `dcim`, `wireless` etc.  
5. Make an API call to retrieve a list of devices in the `Amsterdam` site. Under the `DCIM` section find the `GET /api/dcim/devices/` API call. Click to open it, and then click **Try it out** on the right hand side
6. To filter on only the `amsterdam` site, scroll down and find the `site` parameter, click `Add string item` and enter the site slug of `amsterdam` (lowercase)
7. Scroll further down and click on **Execute** 
8. In the **Responses** section note the full `curl` request and `Request URL` and then scroll down through the **Response Body** to view the data that has been returned from NetBox 

### GraphQL API
1. In the main NetBox Web UI, scroll down to the footer on the left hand side there are 5 icons, and a tool tip appears over each one when you hover over it. Click on the one called **GrappQL API**. This opens a separate browser tab in which you can use the **GraphiQL** utility to build API calls. 
2. Try this out by building a query to retrieve all the devices in the Amsterdam site (`site id: 1`), along with their `ID`, `name` and `platform`. If there is an example query delete it and paste the following: 

```query GetDevicesAtSite {
  site(id: 1) {
    devices {
      id
      name
      platform {
        name
      }
    }
  }
}
```
3. Review the data returned in the panel on the right-hand side. 