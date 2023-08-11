# Render a Device Config using the NetBox REST API

Follow these steps to render the configuration of device `AUSYD01-SW-1` in the REST API. 

## Steps:

### Render Configuration
1. Scroll down to the footer of the Web UI. On the left hand side there are 5 icons, and a tool tip appears over each one when you hover over it. Click on the one called **REST API Documentation**. This opens the Swagger documentation for the REST API in a separate browser tab.  
2. Make an API call to render the configuration of device `AUSYD01-SW-1`. Under the `DCIM` section find the `POST /api/dcim/devices/{id}/render-config/` API call. Click to open it, and then click **Try it out** on the right hand side.
3. In the **Parameters** section note the `id` of the device is required. You can check the `id` of the device in NetBox in the UI by clicking **Devices** > **Devices** > **AUSYD01-SW-1** and in the top-right corner it will say `dcim.device:141`
4. Enter `141` for the `id` parameter, and click **execute**. 
5. In the **Responses** section note the `Request URL` and then scroll down through the **Response Body** to view the data that has been returned from NetBox. The `content` section will contain the device configuration. 