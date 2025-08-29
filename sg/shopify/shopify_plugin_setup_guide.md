# EasyParcel Shopify Integration - App Setup 

---

## Introduction
This guide will walk you through integrating EasyParcel with Shopify using the App Version (Seamless) method. With this integration, you'll have a seamless experience with direct fulfillment from your Shopify App panel. 

---

### Set Up Shopify Integration
#### **Step 1:** [Log in to your EasyParcel account](https://account.easyparcel.com/login?client_id=c575e8cd-aa46-46db-8308-e18d25bb76c6&redirect_uri=https%3A%2F%2Fapp.easyparcel.com%2Feasyaccount%2Fcallback&state=eyJjbGllbnRfaWQiOiI1M2FmYmQzMS05OGI2LTQ3ODctOWYzOC1kMDY5ZGRkN2RiM2QiLCJyZWRpcmVjdF91cmkiOiJodHRwczovL2FwcC5lYXN5cGFyY2VsLmNvbS9sb2dpbi9vYXV0aC9jYWxsYmFjayIsInN0YXRlIjoie30iLCJjb3VudHJ5IjoibXkiLCJsYW5nIjoiZW4ifQ%3D%3D&country=my), go to 'Integration', click on '[Add New Store](https://app.easyparcel.com/my/en/integrations/add/)' and click 'Shopify'.

![Integration Navigation](pictures/SHI1.png) 

---

#### **Step 2:** Select "Plugin Version", and fill in your **Shop Name** and **Shopify Store URL**. Then, click **Next Step** to connect your Shopify store.  

![Step 1 Screenshot](pictures/SHI2.png)  

---

#### **Step 3:** EasyParcel will redirect you to your Shopify store panel. 

![Step 2 Screenshot](pictures/SHI3.png)  

A prompt will appear confirming successful integration. Click **OK**.  

![Step 2 Screenshot](pictures/SHI3.2.png)  

---

#### **Step 4:** Go to your Shopify admin panel → **Apps** → Search for **EasyParcel - Delivery Made Easy** → Click **Install**.  

![Step 3 Screenshot](pictures/SHI4.png)  

---

#### **Step 5:** You’ll be redirected to the EasyParcel settings under the **Getting Started** tab. Read through and click **Start Setup**.  

![Step 4 Screenshot](pictures/SHI5.png)  

---

##### **Step 6:** Go to the **Shipping Setting** tab to fill in your details.  
- Select your shipping country.  
- Insert your **Integration ID** (copied from EasyParcel).  

![Step 5 Screenshot](pictures/SHI6.png)  

Note: Copy your integration ID from here. You can access your integrated stores from '[Your Store](https://app.easyparcel.com/my/en/integrations/your-store/)'. 

![Step 5 Screenshot](pictures/SHI6.2.png)  
---

#### **Step 7:** Review the auto-filled **Sender’s Details**.  
Edit if needed, then click **Save**.  

![Step 6 Screenshot](pictures/SHI7.png)  

---

#### **Step 8:** In Shopify admin:  
- Go to **Settings** → **Checkout**.  
- Under **Shipping address phone number**, choose **Required**.  

⚠️ *If not set, the receiver_contact may be empty → AWB cannot be generated.*  

![Step 7 Screenshot](pictures/SHI8.png)  
![Step 7 Screenshot](pictures/SHI9.png)
![Step 7 Screenshot](pictures/SHI10.png)

---

### Do you shopify growth plan annually billing a above ?
Check out our ***[Live Rate Feature](./live_rates_setup.md)***

## 🚀 Next Steps

Checkout:

[Single Fulfilment](https://github.com/easyparcel/classic-integration-doc/blob/main/sg/shopify/shopify_single_fulfilment.md) | [Bulk Fulfilment](https://github.com/easyparcel/classic-integration-doc/blob/main/sg/shopify/shopify_bulk_fulfilment.md) |  [Auto Fulfilment](https://github.com/easyparcel/classic-integration-doc/blob/main/sg/shopify/shopify_auto_fulfilment.md) |
