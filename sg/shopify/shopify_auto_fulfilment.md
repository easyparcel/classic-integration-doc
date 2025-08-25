# 📦 EasyParcel Auto Fulfilment Guide for Shopify

## 🤔What is Auto Fulfilment?

Auto Fulfilment is a powerful feature that streamlines your shipping process by automatically creating shipping orders when customers place orders on your Shopify store. This hands-off approach saves time and reduces manual work while ensuring orders are processed promptly.

## Setting Up Auto Fulfilment

Follow these steps to enable Auto Fulfilment:

**Step 1: Access the EasyParcel's Shopify App**
   - In your Shopify admin, click on "Apps" and select the "EasyParcel- Delivery Made Easy" Shopify APP.
   - Note: If you haven't installed the EasyParcel Shopify app, learn how to integrate with EasyParcel [here](https://github.com/easyparcel/classic-integration-doc/blob/main/sg/shopify/shopify_plugin_setup_guide.md).
<img width="1328" height="624" alt="image" src="https://github.com/user-attachments/assets/9c5515e3-ea07-4982-8b23-78a585123314" />

**Step 2: Activate Auto Fulfillment Settings**
   - 2.1. Enable Auto Fulfillment: Click on "Auto Fulfillment" within the EasyParcel Shopify app. Change the "Auto Fulfill" setting to "YES."
     <img width="1428" height="622" alt="image" src="https://github.com/user-attachments/assets/6c24af38-709c-4d10-8728-b064f31aaf7a" />
     <img width="1428" height="709" alt="image" src="https://github.com/user-attachments/assets/2581180d-9de8-4fff-8eff-f01ffa55920e" />

   - 2.2. Select Preferred Courier: Choose your preferred courier service for automated order processing.
    <img width="3328" height="1662" alt="image" src="https://github.com/user-attachments/assets/fdacb3ee-b82b-4a97-8499-d2728de653f2" />

   - 2.3. Select Pickup / Dropoff Option: Choose whether you prefer order pickups or drop-offs.
     <img width="1848" height="926" alt="image" src="https://github.com/user-attachments/assets/1d0d109f-a531-4fd4-bc1f-363048d40c82" />

   - 2.4. Click "Save" button.
     <img width="1428" height="689" alt="image" src="https://github.com/user-attachments/assets/5480047c-b36d-4f4b-8593-95469aeccd4b" />


**Step 3: Automated Order Processing and Shipping Label Generation**
Once these settings are configured, new Shopify orders will be automatically processed. Shipping labels (AWBs) will be automatically generated.
   - **Tracking Number:** You can find the tracking number as below image.
     <img width="1328" height="778" alt="image" src="https://github.com/user-attachments/assets/735c7823-d4f8-43b5-a785-516957b17d88" />

   - **Download AWB:** Click "Download AWB" to download and print the shipping labels to attach to your parcels.
     <img width="1328" height="743" alt="image" src="https://github.com/user-attachments/assets/199b6a11-dc44-4322-8bd7-942eefed569f" />

   - **Tracking Status:** You can track the shipping status of your orders as below image too.

**Step 4: You may refer the tracking status of your order here too.**
   <img width="1328" height="622" alt="image" src="https://github.com/user-attachments/assets/836447b7-dd84-4a6c-9682-42c841925d23" />


**Step 5: Auto Fulfillment Log (Optional)**
The auto fulfillment log/history is accessible here.
<img width="1428" height="670" alt="image" src="https://github.com/user-attachments/assets/8c66205a-c67e-4218-ac4e-f6863f2c818f" />


## 🔄 How Auto Fulfilment Works

The Auto Fulfilment process varies depending on your checkout configuration:

### 🎯 Scenario 1: EasyParcel Rates Enabled During Checkout

**Process Flow:**
1. **Customer Places Order** → Customer selects an EasyParcel courier option during checkout
2. **Order Detection** → Plugin automatically detects the new order
3. **Courier Selection Logic** → Plugin attempts to fulfill using:
   - **Primary**: Customer's selected courier service
   - **Fallback**: Default courier service from Auto Fulfilment settings (if customer's choice is unavailable)
4. **Order Completion** → Once fulfilled, download the airway bill from WooCommerce Orders page

### 🎯 Scenario 2: Flat Rate Shipping During Checkout

**Process Flow:**
1. **Customer Places Order** → Customer selects from available flat-rate shipping options
2. **Order Detection** → Plugin automatically detects the new order
3. **Courier Assignment** → Plugin uses the default courier service configured in Auto Fulfilment settings
4. **Order Completion** → Once fulfilled, download the airway bill from WooCommerce Orders page

## 🎯 When to Use Auto Fulfilment

Auto Fulfilment is ideal when you:

- **Want a hands-off experience** with minimal manual intervention
- **Have consistent inventory** with items readily available for shipping
- **Process high order volumes** and need to streamline operations
- **Prefer automated workflows** over manual order processing
- **Want to reduce shipping errors** and processing delays

## 🌟 Benefits

- **Time-saving**: Eliminates manual order processing
- **Consistency**: Ensures all orders are processed using your preferred settings
- **Error reduction**: Minimizes human errors in shipping label creation
- **Improved efficiency**: Faster order turnaround times
- **Better customer experience**: Quicker shipping notifications and tracking

## ⚠️ Important Notes

- Ensure your inventory is accurately maintained for smooth auto-fulfilment
- Regularly check your Auto Fulfilment settings to ensure they match your current shipping preferences
- Monitor processed orders periodically to catch any issues early
- Keep your courier account in good standing to avoid fulfilment interruptions

## 📄 Getting Your Airway Bills

After orders are automatically fulfilled:
1. Go to **WooCommerce > Orders**
2. Find your processed order
3. Click to download the corresponding airway bill
4. Use the airway bill for package labeling and tracking
