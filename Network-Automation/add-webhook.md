# Create and Test a Webhook 

Follow these steps to:
- Create a Webhook that makes an API call to an external system when you create, update or delete an IP address
- Use a free testing website to test that your Webhook is working

## Steps
### Create Webhook

1. You can use a free website to test webhooks, so open a new browser tab and go to: https://webhook.site/ and then copy your unique URL to your clipboard, and leave this tab open. 
2. In the NetBox Web UI, navigate to **Operations** > **Webhooks** and click **+ Add**. 
3. Give it a name and select `IPAM > IP Addresses` for the **Content types** and make sure the `enabled` box is ticked.
4. Under **Events** tick the boxes for `Creations`, `Updates` and `Deletions`. 
5. For the **URL** paste in the value for your unique URL from step 1, leave all other settings as default and then scroll down and click **Create**

### Test Webhook
1. Add a new IP Address, by navigating to **IPAM** > **IP Addresses** and click on **+**. 
2. Enter `10.0.0.20/26` as the IP address, then scroll down and click **Create**, this will trigger the webhook
3. Return to the browser tab that has https://webhook.site/ open and you should see that a new `POST` was received and you will be able to see the raw content of the payload from the API call.
4. Test that deletion also triggers the webhook by deleting the IP address you created in step 1. and checking the `POST` was received again on the test site. 