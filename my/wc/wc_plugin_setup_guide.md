# EasyParcel WooCommerce Integration - Plugin Setup

## Introduction

This guide will walk you through integrating EasyParcel with WooCommerce using the **Plugin Version (Seamless)** method. With this integration, you'll have a seamless experience with shipping rates displayed at checkout and direct fulfillment from your WooCommerce admin panel.

---

## Set Up WooCommerce Integration

**Step 1:** [Log in to your EasyParcel account](https://account.easyparcel.com/login?client_id=c575e8cd-aa46-46db-8308-e18d25bb76c6&redirect_uri=https%3A%2F%2Fapp.easyparcel.com%2Feasyaccount%2Fcallback&state=eyJjbGllbnRfaWQiOiI1M2FmYmQzMS05OGI2LTQ3ODctOWYzOC1kMDY5ZGRkN2RiM2QiLCJyZWRpcmVjdF91cmkiOiJodHRwczovL2FwcC5lYXN5cGFyY2VsLmNvbS9sb2dpbi9vYXV0aC9jYWxsYmFjayIsInN0YXRlIjoie30iLCJjb3VudHJ5IjoibXkiLCJsYW5nIjoiZW4ifQ%3D%3D&country=my), go to 'Integration', click on '[Add New Store](https://app.easyparcel.com/my/en/integrations/add/)' and click 'WooCommerce'.
<img width="1882" height="843" alt="image" src="https://github.com/user-attachments/assets/c5dd408c-cf37-4a62-8af3-d7b99cf8fe80" />


**Step 2:** Fill in your Shop Name and 'Your WooCommerce Store URL'.
<img width="1881" height="829" alt="image" src="https://github.com/user-attachments/assets/0bc67d28-eadf-4895-81ad-9376d61daa04" />


**Step 3:** Choose Plugin version
<img width="1879" height="842" alt="image" src="https://github.com/user-attachments/assets/d10a88fb-bae2-43d6-b3c0-50fbdec0dba8" />


**Step 4:** Click 'Submit'.
<img width="1889" height="850" alt="image" src="https://github.com/user-attachments/assets/b69b783c-b420-49b9-88c4-92aa0011ea50" />


**Step 5:** Copy your integration ID from here. You can also access your integrated stores from '[Your Store](https://app.easyparcel.com/my/en/integrations/your-store/)'.
<img width="1881" height="840" alt="image" src="https://github.com/user-attachments/assets/06f9d152-534a-459a-b5f6-d6845d0dcb3b" />


---

## Install and Activate EasyParcel Plugin in WooCommerce

**Step 1:** Go to your WooCommerce admin panel, click 'Plugin'.

**Step 2:** Search for easyparcel at the Search Plugins.

**Step 3:** Click 'Install Now'.
<img width="1151" height="553" alt="image" src="https://github.com/user-attachments/assets/2b2eacc7-b44c-499c-91a3-5d9b52a5223a" />


**Step 4:** Click 'Activate Plugin'.

<img width="650" height="351" alt="image" src="https://github.com/user-attachments/assets/64391efd-0265-41d9-9cae-eb6e85456646" />

---

## Set Up Rates at Checkout Page for WooCommerce

### Configure EasyParcel Shipping Settings

**Step 1:** Go to your WooCommerce settings, click the 'Shipping tab', then click 'EasyParcel Shipping'. Fill in your details and click 'Save changes'.

> **Note:** After filling out your address details, you may want to recheck it again to confirm the information, as quote rates will be based on the address you provided here.

<img width="1020" height="568" alt="image" src="https://github.com/user-attachments/assets/f46e6aab-d544-4e49-9e1c-e065b5c50983" />

<img width="1023" height="529" alt="image" src="https://github.com/user-attachments/assets/644e5f21-3e0e-47ff-9a07-94fa94f6fa4c" />

<img width="1225" height="141" alt="image" src="https://github.com/user-attachments/assets/39da9cb1-ed74-45dc-9298-dc6e4f2f1ec7" />


### Configure Shipping Zones

**Step 2:** Under the same 'Shipping' tab, click 'Shipping zones' then click 'Add zone'.

> **Note:** You can enjoy multiple zone setups where you can easily classify your customers based on their locations, whether international or domestic. This will help cater to your different online store audience and streamline your checkout process.

<img width="1897" height="820" alt="image" src="https://github.com/user-attachments/assets/70277d5b-46ba-4dbb-a673-1b48f9259722" />


**Step 3:** Give your zone a name, choose zone regions and click 'Add shipping method'.

<img width="1893" height="820" alt="image" src="https://github.com/user-attachments/assets/86b832c0-99f9-4759-89e6-57ff35a03c13" />


**Step 4:** Choose EasyParcel shipping and click 'Continue'.

<img width="1920" height="823" alt="image" src="https://github.com/user-attachments/assets/21080757-b4b8-49d8-8193-a5869114343f" />


**Step 5:** Ensure the 'Enable' button is turned on, then click 'Save changes'.

<img width="1897" height="821" alt="image" src="https://github.com/user-attachments/assets/4cee7dd2-8193-4f43-ab84-8615097102e7" />


### Configure Courier Settings

**Step 6:** Under the same 'Shipping' tab, click 'EasyParcel Courier Setting', then click 'Add Courier Setting'.

> **Note:** This step allows EasyParcel to integrate seamlessly, where it'll unlock access to courier availability, preferred shipping rate options, real-time tracking and more. Please note that it's important that the zones you set in this step match Step 2 above.

<img width="1895" height="820" alt="image" src="https://github.com/user-attachments/assets/fe128086-53ee-409b-94de-f952381c340d" />

**Step 7:** Fill in Zone Name, Destination and click 'Add courier service'.

<img width="1897" height="821" alt="image" src="https://github.com/user-attachments/assets/18224199-09a9-42e0-99cf-c042ccda9fd5" />


**Step 8:** Choose your preferred courier service in the drop-down.

<img width="1893" height="818" alt="image" src="https://github.com/user-attachments/assets/c413f248-3e73-45b3-894e-700c1748bf5d" />


### Courier Service Options:

**i) All couriers**
> **Note:** Any couriers that fit and are available for the destinations during the checkout process will appear for your customers to choose.

**ii) Specific courier**
> **Note:** You can choose a specific courier that you prefer. Then, in the 'Courier Display Name', you may choose what name you'd like your customers to see at the checkout.

**iii) Cheapest Courier**
> **Note:** This will streamline your process of choosing couriers one by one. By choosing this option, the system will automatically find the cheapest courier to deliver to the customer's destination during checkout.

<img width="1893" height="818" alt="image" src="https://github.com/user-attachments/assets/880ce007-b4c4-455c-9941-082db9578031" />


### Configure Shipping Rate Settings

**Step 9:** Choose your preferred shipping rate setting, then click 'Save changes'.

**i) EasyParcel Member Rate**
> **Note:** You may choose this option if you would like your customers to view and pay the shipping rate based on your EasyParcel membership rate only.

**ii) Add on EasyParcel Member Rate**
> **Note:** You may choose this option if you would like your customers to view and pay the shipping rate of your EasyParcel membership rate plus an amount that you can set up. You may choose 'Add On By Amount' or 'Add On By Percentage' and state the value in the space provided.

**iii) Flat Rate**
> **Note:** You may choose this option if you would like to simply set up a fixed amount for the shipping fee that your customers can pay at the checkout.

<img width="1893" height="824" alt="image" src="https://github.com/user-attachments/assets/3da88cd2-f992-471f-a727-ae8265eaec04" />


---

## Fulfillment on WooCommerce
There's three ways to fulfil orders using easyparcel plugin

### Single Fulfillment
Manual fulfilment with most control and flexibility

Check out on [Single fulfilment](./wc_single_fulfilment.md)


### Bulk Fulfillment
Fulfil orders in bulk great for large order amounts

Check out on [Bulk fulfilment](./wc_bulk_fulfilment.md)


### Auto Fulfillment 
Most hands of method

Check out on [Auto fulfilment](./wc_auto_fulfilment.md)

---

## Conclusion

You've successfully set up EasyParcel WooCommerce integration using the Plugin Version (Seamless)! Your customers will now see real-time shipping rates at checkout, and you can fulfill orders directly from your WooCommerce admin panel. 

If you have any questions or need further assistance, [check out our other articles](https://helpcentre-my.easyparcel.com/support/home) or reach out to our friendly support team. We're happy to help you every step of the way!
