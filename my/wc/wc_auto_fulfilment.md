# 📦 EasyParcel Auto Fulfilment Guide for WooCommerce

## 🤔What is Auto Fulfilment?

Auto Fulfilment is a powerful feature that streamlines your shipping process by automatically creating shipping orders when customers place orders on your WooCommerce store. This hands-off approach saves time and reduces manual work while ensuring orders are processed promptly.

## Setting Up Auto Fulfilment

Follow these steps to enable Auto Fulfilment:

1. **Navigate to Auto Fulfilment Settings**
   - Go to the EasyParcel tab in your WooCommerce admin panel

2. **Select to Auto Fulfilment Settings**
   - Select "Auto Fulfilment" from the menu

3. **Enable Auto Fulfilment**
   - Change the Auto Fulfilment setting to "Yes"

4. **Choose Your Preferred Courier**
   - Select your default courier service from the dropdown menu

5. **Select Service Type**
   - Choose between:
     - **Drop Off Service**: You bring packages to a designated location
     - **Pick Up Service**: Courier collects packages from your location

6. **Configure Drop Off Location** (if applicable)
   - If you selected Drop Off Service, choose your preferred drop-off point from the available locations

7. **Save Settings**
   - Click "Save" to apply your configuration
     
<img width="1237" height="592" alt="image" src="https://github.com/user-attachments/assets/14e85fee-c820-44ac-97cb-4e5e6f16999a" />



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
