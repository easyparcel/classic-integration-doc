# EasyParcel Shopify Integration - App Setup 

---

## Introduction
This guide will walk you through integrating EasyParcel with Shopify using the App Version (Seamless) method. With this integration, you'll have a seamless experience with direct fulfillment from your Shopify App panel. 

---

### Set Up Shopify Integration
**Step 1:** [Log in to your EasyParcel account](https://account.easyparcel.com/login?client_id=c575e8cd-aa46-46db-8308-e18d25bb76c6&redirect_uri=https%3A%2F%2Fapp.easyparcel.com%2Feasyaccount%2Fcallback&state=eyJjbGllbnRfaWQiOiI1M2FmYmQzMS05OGI2LTQ3ODctOWYzOC1kMDY5ZGRkN2RiM2QiLCJyZWRpcmVjdF91cmkiOiJodHRwczovL2FwcC5lYXN5cGFyY2VsLmNvbS9sb2dpbi9vYXV0aC9jYWxsYmFjayIsInN0YXRlIjoie30iLCJjb3VudHJ5IjoibXkiLCJsYW5nIjoiZW4ifQ%3D%3D&country=my), go to 'Integration', click on '[Add New Store](https://app.easyparcel.com/my/en/integrations/add/)' and click 'Shopify'.

![Integration Navigation](pictures/SHI1.png) 

---

**Step 2:** Fill in your **Shop Name** and **Shopify Store URL**. Then, click **Next Step** to connect your Shopify store.  

![Step 1 Screenshot](pictures/SHI2.png)  

---

**Step 3:** EasyParcel will redirect you to your Shopify store panel. 

![Step 2 Screenshot](pictures/SHI3.png)  

A prompt will appear confirming successful integration. Click **OK**.  

![Step 2 Screenshot](pictures/SHI3.2.png)  

---

**Step 4:** Go to your Shopify admin panel → **Apps** → Search for **EasyParcel - Delivery Made Easy** → Click **Install**.  

![Step 3 Screenshot](pictures/SHI4.png)  

---

**Step 5:** You’ll be redirected to the EasyParcel settings under the **Getting Started** tab. Read through and click **Start Setup**.  

![Step 4 Screenshot](pictures/SHI5.png)  

---

**Step 6:** Go to the **Shipping Setting** tab to fill in your details.  
- Select your shipping country.  
- Insert your **Integration ID** (copied from EasyParcel).  

![Step 5 Screenshot](pictures/SHI6.png)  

Note: Copy your integration ID from here. You can access your integrated stores from '[Your Store](https://app.easyparcel.com/my/en/integrations/your-store/)'. 

![Step 5 Screenshot](pictures/SHI6.2.png)  
---

**Step 7:** Review the auto-filled **Sender’s Details**.  
Edit if needed, then click **Save**.  

![Step 6 Screenshot](pictures/SHI7.png)  

---

**Step 8:** In Shopify admin:  
- Go to **Settings** → **Checkout**.  
- Under **Shipping address phone number**, choose **Required**.  

⚠️ *If not set, the receiver_contact may be empty → AWB cannot be generated.*  

![Step 7 Screenshot](pictures/SHI8.png)  
![Step 7 Screenshot](pictures/SHI9.png)
![Step 7 Screenshot](pictures/SHI10.png)

---

## How to fulfil Shopify orders via EasyParcel Shopify APP?

### 1: How to fulfill Shopify single orders?

**Step 1:** After a customer places an order in your Shopify store, ensure the order's payment status is "Paid.

<img width="1328" height="313" alt="image" src="https://github.com/user-attachments/assets/1dc077b5-e42c-4c6b-86da-462bcb8542cb" />

**Step 2:** In your Shopify admin, click on "Apps" and select the "EasyParcel- Delivery Made Easy" app.

**Note:** If you haven't yet installed the EasyParcel Shopify app, refer to these instructions to learn more about integrating with EasyParcel.

<img width="1328" height="624" alt="image" src="https://github.com/user-attachments/assets/ce769abb-a6ee-4317-bd58-ed984006b630" />

**Step 3:** Sync and Select Order:

- Click on the "Orders" tab (or similar, depending on the app's interface).
- Click "Sync Orders from Shopify" to refresh the list of orders.
- Click on the order number you wish to fulfill.

<img width="1328" height="793" alt="image" src="https://github.com/user-attachments/assets/a8b8381a-fa5c-4fa7-82b5-04765c4b4fbf" />

**Step 4:** Fulfill Order:

- Enter the quantity of items you wish to ship.
- Click "Get Quote" to view available courier options and rates.
- Select your preferred courier service.
- Click "Fulfill Order" to complete the shipping process.

<img width="1328" height="1055" alt="image" src="https://github.com/user-attachments/assets/557e220b-4a5b-466e-83a2-8689fe2c73dd" />

**Note:** You can choose drop-off service, you may choose your preferred drop-off location here.

<img width="1897" height="824" alt="image" src="https://github.com/user-attachments/assets/afaa2027-5c55-48ae-bcc0-9f858a979f7c" />

**Step 5:** AWB auto-generated

- You can get the tracking number here
- Click 'Download AWB' to attach them on your parcels
- You may refer the tracking status of your order here too.

<img width="1328" height="622" alt="image" src="https://github.com/user-attachments/assets/e6f79407-0f3c-4c8a-b2cd-fd02cc024624" />

### 2: How to fulfill multiple Shopify orders at once?

**Step 1:** After a customer places an order in your Shopify store, ensure the order's payment status is "Paid.

<img width="1328" height="313" alt="image" src="https://github.com/user-attachments/assets/acb4654b-c980-4332-bd3e-e5f2cfed9d94" />

**Step 2:** In your Shopify admin, click on "Apps" and select the "EasyParcel- Delivery Made Easy" app.

**Note:** If you haven't yet installed the EasyParcel Shopify app, refer to these instructions to learn more about integrating with EasyParcel.

<img width="1328" height="624" alt="image" src="https://github.com/user-attachments/assets/d6b7f0f4-a2e0-46c4-ba41-c4b6d4b8bb04" />

**Step 3:** Select Orders

- In the "Orders" section, apply filters to find the orders you want to fulfill.
- Select the checkbox next to each order.
- Click "Fulfill Orders.

<img width="1328" height="750" alt="image" src="https://github.com/user-attachments/assets/e3c19b75-2bf3-4907-a207-0c21d557370e" />

**Step 4:** Choose Courier and Pickup Date

- A pop-up window will appear. 
- Select your desired courier and pickup date. 
- Click "Submit."

<img width="1328" height="743" alt="image" src="https://github.com/user-attachments/assets/4d3fe764-9255-4013-be03-2ec288c7eb0e" />

**Step 5:** AWB Generation and Tracking

- Your Air Waybills (AWBs) will be generated automatically.
- You can find the tracking numbers on "Tracking Number" coulumn.
- Click "Download AWB" to print and attach the AWBs to your parcels.

<img width="1328" height="778" alt="image" src="https://github.com/user-attachments/assets/a01ae5b3-d9ea-452e-b32e-5d49c598f2b4" />
<img width="1328" height="743" alt="image" src="https://github.com/user-attachments/assets/93239a7b-855f-4e19-86d5-5363248d55e6" />

**Step 6:** You may refer the tracking status of your order here

<img width="1328" height="622" alt="image" src="https://github.com/user-attachments/assets/99a770de-ebb1-4183-ab51-71d6edf9034c" />

---

## Conclusion

You've successfully set up EasyParcel Shopify integration using the App Version (Seamless)! You will now can fulfill orders directly from your Shopify App panel. 

If you would like to add live rates to your Shopify checkout page, kindly refer to the following guide [How to Add Live Shipping Rates at Checkout for Shopify](https://github.com/easyparcel/classic-integration-doc/blob/main/sg/shopify/live_rates_setup.md).

If you have any questions or need further assistance, [check out our other articles](https://helpcentre-my.easyparcel.com/support/home) or reach out to our friendly support team. We're happy to help you every step of the way! 

