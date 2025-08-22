# How to Resolve Missing Phone Numbers in Shopify Shipping Address via EasyParcel Integration

## Error Message

When doing fulfillment in EasyParcel application, you may encounter this error:

> ⚠️ **Invalid mobile number in receiver's contact.**

*[Image placeholder: Error message screenshot]*

## Solution Steps

### Step 1: Check Shipping Address in EasyParcel

Please check the shipping address section of your order when it syncs to EasyParcel, as many customers often overlook filling in the phone number. For your reference, the attached image from the EasyParcel application shows how it will appear when fulfilling an order through EasyParcel.

**Example of missing phone number:**
```
Shipping Address
Kuala Lumpur Malaysia
55100
+6011  [← Phone field is incomplete/invalid]

Billing Address
Kuala Lumpur Malaysia
55100
+6011
```

*[Image placeholder: EasyParcel shipping address screenshot]*

### Step 2: Navigate to Shopify Orders

Navigate to your Shopify Orders page, then click on the specific order that has the phone number issue.

### Step 3: Edit Shipping Address

Click on the three dots (**…**) to open a menu with three options, then select **"Edit shipping address."**

*[Image placeholder: Shopify order details with three dots menu]*

### Step 4: Enter Phone Number

Scroll down to the **"Phone"** field, enter your customer's phone number, and click **"Save."**

Once saved, you can proceed to fulfill the order again with EasyParcel, and it should go through successfully.

*[Image placeholder: Edit shipping address dialog with phone field]*

## Prevention (Recommended)

### Step 5: Make Phone Number Required

To prevent this issue from occurring, we recommend making the phone number field a required field in your Shopify settings.

**To set up:**
1. Go to the **Shopify admin panel**
2. Click **Settings**
3. Click **Checkout**
4. Ensure the **Phone number under Shipping address** is marked as **Required**

**Shipping address phone number options:**
- ⚪ Don't include
- ⚪ Optional  
- 🔘 **Required** ← Select this option

*[Image placeholder: Shopify checkout settings with phone number options]*

## Summary

By following these steps, you can resolve missing phone number issues and prevent them from occurring in future orders. Making the phone number field required ensures all orders will have the necessary contact information for successful EasyParcel fulfillment.
