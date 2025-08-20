# EasyParcel WooCommerce Integration - Plugin Setup

## Introduction

This guide will walk you through integrating EasyParcel with WooCommerce using the **Plugin Version (Seamless)** method. With this integration, you'll have a seamless experience with shipping rates displayed at checkout and direct fulfillment from your WooCommerce admin panel.

---

## Set Up WooCommerce Integration

**Step 1:** [Log in to your EasyParcel account](https://account.easyparcel.com/login?client_id=c575e8cd-aa46-46db-8308-e18d25bb76c6&redirect_uri=https%3A%2F%2Fapp.easyparcel.com%2Feasyaccount%2Fcallback&state=eyJjbGllbnRfaWQiOiI1M2FmYmQzMS05OGI2LTQ3ODctOWYzOC1kMDY5ZGRkN2RiM2QiLCJyZWRpcmVjdF91cmkiOiJodHRwczovL2FwcC5lYXN5cGFyY2VsLmNvbS9sb2dpbi9vYXV0aC9jYWxsYmFjayIsInN0YXRlIjoie30iLCJjb3VudHJ5IjoibXkiLCJsYW5nIjoiZW4ifQ%3D%3D&country=my), go to 'Integration', click on '[Add New Store](https://app.easyparcel.com/my/en/integrations/add/)' and click 'WooCommerce'.

**Step 2:** Fill in your Shop Name and 'Your WooCommerce Store URL'.

**Step 3:** Choose Plugin version

**Step 4:** Hit the 'Version to download' drop-down to choose the latest version available.

**Step 5:** Hit 'Download'.

**Step 6:** Click 'Submit'.

**Step 7:** Copy your integration ID from here. You can also access your integrated stores from '[Your Store](https://app.easyparcel.com/my/en/integrations/your-store/)'.

---

## Install and Activate EasyParcel Plugin in WooCommerce

**Step 1:** Go to your WooCommerce admin panel, click 'Plugin'.

**Step 2:** Search for easyparcel at the Search Plugins.

**Step 3:** Click 'Install Now'.

**Step 4:** Click 'Activate Plugin'.

---

## Set Up Rates at Checkout Page for WooCommerce

### Configure EasyParcel Shipping Settings

**Step 1:** Go to your WooCommerce settings, click the 'Shipping tab', then click 'EasyParcel Shipping'. Fill in your details and click 'Save changes'.

> **Note:** After filling out your address details, you may want to recheck it again to confirm the information, as quote rates will be based on the address you provided here.

### Configure Shipping Zones

**Step 2:** Under the same 'Shipping' tab, click 'Shipping zones' then click 'Add zone'.

> **Note:** You can enjoy multiple zone setups where you can easily classify your customers based on their locations, whether international or domestic. This will help cater to your different online store audience and streamline your checkout process.

**Step 3:** Give your zone a name, choose zone regions and click 'Add shipping method'.

**Step 4:** Choose EasyParcel shipping and click 'Continue'.

**Step 5:** Ensure the 'Enable' button is turned on, then click 'Save changes'.

### Configure Courier Settings

**Step 6:** Under the same 'Shipping' tab, click 'EasyParcel Courier Setting', then click 'Add Courier Setting'.

> **Note:** This step allows EasyParcel to integrate seamlessly, where it'll unlock access to courier availability, preferred shipping rate options, real-time tracking and more. Please note that it's important that the zones you set in this step match Step 2 above.

**Step 7:** Fill in Zone Name, Destination and click 'Add courier service'.

**Step 8:** Choose your preferred courier service in the drop-down.

### Courier Service Options:

**i) All couriers**
> **Note:** Any couriers that fit and are available for the destinations during the checkout process will appear for your customers to choose.

**ii) Specific courier**
> **Note:** You can choose a specific courier that you prefer. Then, in the 'Courier Display Name', you may choose what name you'd like your customers to see at the checkout.

**iii) Cheapest Courier**
> **Note:** This will streamline your process of choosing couriers one by one. By choosing this option, the system will automatically find the cheapest courier to deliver to the customer's destination during checkout.

### Configure Shipping Rate Settings

**Step 9:** Choose your preferred shipping rate setting, then click 'Save changes'.

**i) EasyParcel Member Rate**
> **Note:** You may choose this option if you would like your customers to view and pay the shipping rate based on your EasyParcel membership rate only.

**ii) Add on EasyParcel Member Rate**
> **Note:** You may choose this option if you would like your customers to view and pay the shipping rate of your EasyParcel membership rate plus an amount that you can set up. You may choose 'Add On By Amount' or 'Add On By Percentage' and state the value in the space provided.

**iii) Flat Rate**
> **Note:** You may choose this option if you would like to simply set up a fixed amount for the shipping fee that your customers can pay at the checkout.

---

## Fulfillment on WooCommerce

### Single Fulfillment

**Step 1:** To fulfill your order, simply click on your order details.

**Step 2:** Check on the shipping details and click 'Fulfill Order'.

**Step 3:** Once fulfilled, you can download the shipment Air Waybill (AWB).

### Bulk Fulfillment

**Step 1:** Select the orders you want to fulfil, click the drop-down button, choose 'Order Fulfillment' then click 'Apply'.

**Step 2:** Choose your preferred couriers in the drop-down.

**Step 3:** Choose Drop off/Pick Up date and click 'Fulfill Order'.

**Step 4:** Select the orders you want AWB in bulk, in the drop-down, click 'Download Bulk AWBs' and hit 'Apply'.

> **Note:** The status will automatically turn to 'Completed' once done.

### Auto Fulfillment

**Step 1:** Go to easyparcel auto fulfilment settings tab.

**Step 2:** Turn Auto Fulfil to Yes.

**Step 3:** Choose your preferred couriers in the drop-down.

**Step 4:** Choose Drop off/Pick Up date and click 'Fulfill Order'.

**Step 5:** Select a drop off point if selected drop off point.

**Step 6:** Cick Save.

> **Note:** New incoming order will be auto fulfilled base on customer selected while fallback to the preffered courier if not avaliable.
> 
> For information regarding auto fulfilment may visits here **here**
---

## Conclusion

You've successfully set up EasyParcel WooCommerce integration using the Plugin Version (Seamless)! Your customers will now see real-time shipping rates at checkout, and you can fulfill orders directly from your WooCommerce admin panel.

If you have any questions or need further assistance, [check out our other articles](https://helpcentre-my.easyparcel.com/support/home) or reach out to our friendly support team. We're happy to help you every step of the way!
