# Q&As [Shopify]

## Technical Questions

<details>
<summary><strong>Q: Not able to choose the courier.</strong></summary>

## Situation 1: Duplicate Billing Address
- If your order shows **two identical billing addresses** and no shipping address:  
  1. Verify your order details.  
  2. Update and set one of the addresses as the shipping address.  
  3. After the update, your order will display both billing and shipping addresses correctly.  

---

## Situation 2: Missing Shipping Address
- If your order shows **only a billing address but no shipping address**:  
  1. Confirm if your billing address should also be the same as your shipping address.  
  2. If both of the address is the same, duplicated the address and updated it as the shipping address.  

---

## Situation 3: Two Different Billing Addresses
- If your order shows **two different billing addresses**:  
  1. Confirm which one should be used as the shipping address.  
  2. Once confirmed, updated the address as the shipping address in the system.

</details>

<details>
<summary><strong>Q: Customer is having Import issues: "Receiver Contact is Empty"</strong></summary>
  
[Edit shipping address > phone number] is empty. 

<img width="1280" height="596" alt="image" src="https://github.com/user-attachments/assets/d3aecd5a-6ca4-45bc-908b-d0a21aa4d959" />

**Note:** [Edit contact information > phone number] is not the one used

**To Do:** ask the customer to enable require shipping phone number in checkout to avoid this issue

A tip for checking: 
*Contact number in the contact information section will not be retrieved by our system* 
*Only the mobile number in the shipping address will be retrieved to our system*
In their app if the order details Shipping Address don't have phone number means it is empty

<img width="1280" height="653" alt="image" src="https://github.com/user-attachments/assets/2dea6ea7-46f2-42e3-9311-78d9948df6b0" />

[Full documentation about this issue](https://easyparcel.sg.larksuite.com/docx/PSQ8dTBTuota4oxHeRuldxHzgSe)


</details>

<details>
<summary><strong>Q: Error message shows when click on the Download Air Waybill</strong></summary>

<img width="1280" height="588" alt="image" src="https://github.com/user-attachments/assets/4c4a3891-5be1-4f14-a62b-52435ce5cb82" />

**A:** The order need to be fulfilled first in order to get the AWB.

</details>

<details>
<summary><strong>Q: During import, the order has been proceeded, but failed due to some details are empty.</strong></summary>

<img width="1280" height="540" alt="image" src="https://github.com/user-attachments/assets/8a8a5f63-ef21-4b7e-b0cd-ee50e333f270" />

**A:** The error message will indicate the reason why the order could not be imported, and you can resolve the issue based on the details provided in the error message.

</details>

<details>
<summary><strong>Q: No Tracking URL/ No downloadable AWB after fulfillment</strong></summary>



</details>

<details>
<summary><strong>Q: Order cant import to EP website</strong></summary>

<img width="2000" height="3556" alt="image" src="https://github.com/user-attachments/assets/619bb77f-9f44-446c-ac42-7789f91280ae" />

**A**: Check if the URL are matched with your domain name in Shopify. For example:

<img width="1280" height="341" alt="image" src="https://github.com/user-attachments/assets/21821485-3181-42c5-848d-1d8ab4ef770b" />

As a lot of customers mistakenly put their admin panel url instead

</details>

<details>
<summary><strong>Q: Changed the product weight but weight still the same in Shopify app</strong></summary>

**A:** Due to Shopify design, products added to an order will remain its weight value, it will only use the newly set weight for new orders. However, there is a way to update the weight for existing orders. By removing the item from the order and re-adding it back.

<img width="1280" height="649" alt="image" src="https://github.com/user-attachments/assets/5da783a6-f9e0-4521-ab30-8c42ba63a9c0" />

</details>

<details>
<summary><strong>Q: Order not showing up in app</strong></summary>

**A1:** Order was made before the easyparcel app was installed
   
**A2:** Orders older than 30 days will not show
   
**A3:** May clear browser cache and try again.

</details>

<details>
<summary><strong>Q: Unable to import if weight is 0kg</strong></summary>

**A:** If you are unable to import an order into the EasyParcel website or no order is found in the EasyParcel App, kindly check the product weight. If the product weight is set to 0kg, the order will not be able to imported or displayed in the EasyParcel App.

</details>

<details>
<summary><strong>Q:How does a seller get the EasyParcel Integration ID?</strong></summary>

### Step 1: Get EasyParcel Integration ID

- Log in to EasyParcel and obtain your Integration ID from EasyParcel Website.

### Step 2: Configure Integration Settings

- Go to your store's EasyParcel Integration Settings page.
- Enter the Integration ID and required address details, then save the settings.

### Step 3: API Endpoint Authentication

- Authentication: Use the auth key from your EasyParcel account.
- API Field: Enter the Integration ID you set in the integration settings.

</details>

<details>
<summary><strong>Q:What is the difference between pick point and send point?</strong></summary>

**A:** The pick_point refers to the sender's drop-off location, and the send_point refers to the receiver's pickup location.
</details>

<details>
<summary><strong>Q:If already integrate with Shopify but still get can't import Error message</strong></summary>
  
<img width="1158" height="703" alt="image" src="https://github.com/user-attachments/assets/3cd945c0-05fa-4a37-8607-dbb1e8f3411e" />

### Step 1: You can uninstall easy parcel application in shopify

<img width="1280" height="251" alt="image" src="https://github.com/user-attachments/assets/6e5b76e0-b91e-498b-b56c-ba8e6f65088b" />

### Step 2: Go to the portal page and search for the integration section and remove your shopify integration

<img width="1280" height="330" alt="image" src="https://github.com/user-attachments/assets/485b04aa-457d-476b-aae4-49c93277b1a7" />

### Step 3: Reintegrate again with the same step

[Shopify_Import_Integration_setup](https://github.com/easyparcel/classic-integration-doc/blob/main/sg/shopify/shopify_import_integration_setup.md)

</details>

<details>
<summary><strong>Q:Import order but not synced to portal</strong></summary>

**Situation 1**
### Step 1: Reauthourize the Shopify App through EasyParcel website setting, after click 'edit' in portal side 
<img width="1280" height="424" alt="image" src="https://github.com/user-attachments/assets/2720863c-6f7d-4486-94d7-92f57b38d1a8" />

### Step 2: Update the store information and click on the 'save'. It will prompt you to Shopify webpage to allow authorization with EasyParcel and press 'allow'.
<img width="1280" height="1041" alt="image" src="https://github.com/user-attachments/assets/c1f93f9a-ac25-4db8-901e-7fb8a2a45fce" />

**Situation 2: Suddenly cant import**

<img width="1280" height="628" alt="image" src="https://github.com/user-attachments/assets/c704bbc5-50ea-4b0e-8d6e-aa246c0c6fc7" />

**A:** The issue may be caused by an incorrect URL link, which can be resolved by updating it to the correct store link.

</details>

<details>
<summary><strong>Q: It's fine to use customer's consumer key, consumer secret and shop url (if they have provided) to test integration on our own account when customer is facing import issue</strong></summary>

This is acceptable for troubleshooting purposes.

</details>

<details>
<summary><strong>Q: If the customer shop url, consumer secret and consumer key is correct but still failed to import the order</strong></summary>

**A:** Suggest them to delete the integration and integrate again to see if the issue is solved

</details>

<details>
<summary><strong>Q: If there is anyway to set a specific amount for delivery for our customers based on weight? For example, 1kg - 5kg will be Rm5, 5.1kg to 10kg will be Rm10</strong></summary>

**A:** No. Currently our plugin does not have this feature

</details>

<details>
<summary><strong>Q: Some orders can't be imported to the system</strong></summary>

**Requirements for order import:**
- Order generated within 7 days
- Order status is processing
- Make sure product weight value is not empty

</details>

<details>
<summary><strong>Q: Why is the parcel dimensions in API log different from the dimensions set in WooCommerce product</strong></summary>

**A:** Check the unit set in WooCommerce. If it is not cm, it will be converted and shown in cm in the API log.

</details>

<details>
<summary><strong>Q: Unable to edit courier services</strong></summary>

The courier services are can't be edited once you save changes, you may need to delete to add new courier service to change

Courier service type only able to be select when adding new service

</details>

<details>
<summary><strong>Q: "Courier Setting > Locations not covered by your other zones"</strong></summary>

**Solution:**
- Check their version, if using legacy (e.g. v1.6.8.18) ask them to switch to
- Check if this option is enabled

</details>

<details>
<summary><strong>Q: Courier Setting > Locations not covered by your other zones (for WooCommerce official plugin in extension)</strong></summary>

**Solution:**
Try switching to the plugin from our portal instead

Switch from EasyParcel Shipping from this to our version

</details>

<details>
<summary><strong>Q: No courier service to select when trying to fulfil order</strong></summary>

**Solutions:**
- Check api log, could be because weight is 0, no shipping postcode, etc
- Check EasyParcel Shipping page. If not filled up, API will not get any requests

</details>

<details>
<summary><strong>Q: Have testing / demo / sandbox environment to test?</strong></summary>

**A:** No, our plugin is only for live use.

</details>

<details>
<summary><strong>Q: Unable to find Qxpress Courier service on Courier Settings</strong></summary>

Due to recent Qxpress brand name changes, Qxpress will no longer be available as a courier option and has been updated to Tracxlogis. To change from Qxpress to Tracxlogis:

1. Go to WooCommerce -> Settings -> Shipping -> EasyParcel Courier Setting
2. Select and Edit Zones that previously selected Qxpress as Courier Service
3. Delete the Qxpress Courier
4. Add new courier services
5. Select Tracxlogis as Courier Service
6. Select the rate settings preferred
7. Save Changes.

</details>

<details>
<summary><strong>Q: No courier show up, credit balance = 0.00, all API related information not available, no API log</strong></summary>

**Check if its status 403 (Forbidden) issue:**

```php
// easiest way to check is using easyparcel shipping settings page
// in check credit balance api call, log the response code to check

wc_get_logger()->info(wp_remote_retrieve_response_code($r));
// then check in woocommerce status -> log
```

**To suggest fix to customer:**
https://www.cloudways.com/blog/wordpress-403-forbidden-error/#fixes

</details>

<details>
<summary><strong>Q: Why can I retrieve all couriers using my API key in log.php but only see cargo couriers displayed?</strong></summary>

If the volumetric weight calculated using the volumetric calculator is higher than the actual weight, the volumetric weight will be used as the final weight.

</details>

<details>
<summary><strong>Q: If shipping courier, flat rate can't show at checkout</strong></summary>

**A:** But it got show at api log, It mind due to user woocommerce problem so it won't display any rate even if is a flat rate

</details>

<details>
<summary><strong>Q: Undefined array error appears at checkout page</strong></summary>

**Solution:**
Ask customer to turn off debug mode on wp-config.php file

Sample code:
```php
define( 'WP_DEBUG', false );
```

**Reference article:**
https://developer.wordpress.org/advanced-administration/debug/debug-wordpress/

</details>

<details>
<summary><strong>Q: Unable to show courier even if all settings are correct</strong></summary>

It may be due to the easy parcel courier setting section where one zone is everywhere. This will create cache and block the country showing courier delete that everywhere zone then the problem will be fixed.

</details>

<details>
<summary><strong>Q: Unable to find Singpost in courier setting</strong></summary>

Due to recent Singpost brand name changes, Singpost will no longer be available as a courier option and has been updated to Speedpost. To change from Singpost to Speedpost:

1. Go to WooCommerce -> Settings -> Shipping -> EasyParcel Courier Setting
2. Select and Edit Zones that previously selected Singpost as Courier Service
3. Delete the Singpost Courier
4. Add new courier services
5. Select Speedpost as Courier Service
6. Select the rate settings preferred
7. Save Changes.

May refer to trackxlogis document or you can re-add by shipping zone edit -> add courier -> choose speedpost courier -> then save changes

</details>

<details>
<summary><strong>Q: Does Auto fulfilment courier support multiple couriers at the same time</strong></summary>

If you allow customer to select our courier during check page then it will fulfil based on customer selected courier, while if using custom rate then currently  only able to select one

</details>


<details>
<summary><strong>Q: Does WooCommerce mobile app support our plugin</strong></summary>

**A:** No, WooCommerce mobile app does not support our plugin, to fulfil the order via woocommerce plugin, will need to use Web version of woocommerce.

To access Web version of woocommerce through app you follow as such:
App dashboard, bottom right button -> select WC admin

</details>

<details>
<summary><strong>Q: How is the item with volumetric weight is calculated</strong></summary>

**How We Handle Package Dimensions for Multiple Items**

When processing orders with multiple items, we don't simply add up all the dimensions. Instead, we use a **smart packaging algorithm** that optimizes the final package size to avoid excessive volumetric weight charges.

**Our Dimension Calculation Logic:**

**For each item in the order:**
- We track both the **maximum** dimension and **sum** of dimensions for length, width, and height
- Each dimension is converted to centimeters and validated

**Smart Packaging Algorithm:**

We calculate three sums: sumLength, sumWidth, sumHeight
Then we find the smallest sum among these three
Final dimensions are determined as:
- If sumLength is smallest → Use: sumLength × maxWidth × maxHeight
- If sumWidth is smallest → Use: maxLength × sumWidth × maxHeight  
- If sumHeight is smallest → Use: maxLength × maxWidth × sumHeight

**Why This Approach?**

**Problem:** Simply adding all dimensions (L+L+L, W+W+W, H+H+H) would create unrealistically large packages and result in very high volumetric weight charges.

**Solution:** Our algorithm assumes items can be packed efficiently by:
- **Stacking** along the smallest total dimension
- **Using the largest single item size** for the other two dimensions

**Example:**

If you order 3 identical boxes (10cm × 5cm × 3cm each):
- Simple sum would be: 30cm × 15cm × 9cm = 4,050 cm³
- Our smart algorithm: 30cm × 5cm × 3cm = 450 cm³ *(stacking along length)*

This represents realistic packaging where items are stacked efficiently, resulting in more accurate shipping costs and better customer experience.

**Benefits:**
- ✅ **Lower shipping costs** due to realistic volumetric weight
- ✅ **Accurate courier quotations**
- ✅ **Efficient packaging** recommendations
- ✅ **Prevents overcharging** customers

**Basically:**
W/L/H = width length height
Smallest sum of either W/L/H × the largest W/L/H × the W/L/H

</details>

<details>
<summary><strong>Q: Customer wants to split 1 order into few shipment</strong></summary>

We recommend that sellers use this plugin. However, we advise them to mark up their shipping fees. This is because the plugin cannot collect multiple shipping fees from buyers, and the order can only be split once the buyer has completed the payment.


<img width="1600" height="766" alt="asynccode" src="https://github.com/user-attachments/assets/fef4794f-2f20-44d2-bd50-d3acac6257c0" />


</details>

---

## Operation Questions

<details>
<summary><strong>Q: Will order fulfill status changed after the order is fulfilled in WooCommerce?</strong></summary>

When importing an order to the EP dashboard and fulfilling it, the order status in WooCommerce will not update to "complete." The order status will be updated to "complete" only when the order is fulfilled in WooCommerce.

If the customer's EP credit is not enough, the order could not be made and the status will not be updated. Additionally, if the customer pays for the order shipping on the EP dashboard, the order status will not be updated to "Complete" automatically. The customer will need to manually change the status.

</details>

<details>
<summary><strong>Q: Does WooCommerce plugin integration provide COD service?</strong></summary>

**A:** No, COD service is not provided in WooCommerce plugin version. If the customer wishes to use COD, they might have to use the Simple Version, import and fulfill their orders through EasyParcel.

</details>

<details>
<summary><strong>Q: What to request WooCommerce login from the customer if not able to check on the log.</strong></summary>

**A:** Those are the required data:
- WordPress login URL:
- Username:
- Password:

</details>

<details>
<summary><strong>Q: Shipping rate is too high, courier fee charges not according what the product weight resulting showing higher charges.</strong></summary>

**A:** Check the dimension of the product. Please remove the product dimensions and only include the weight. If the product has variations, the dimensions of those variations also need to be specified.

After making any changes, it is necessary to clear the WooCommerce cart and refresh the page before testing the modifications. This ensures that you begin with a clean cart and allows the changes to be properly reflected throughout the shopping process.

</details>

<details>
<summary><strong>Q: Can I enable WhatsApp Tracking in WooCommerce plugin integration?</strong></summary>

No, WhatsApp tracking currently (22nd August 2024) only available on simple integration

</details>

<details>
<summary><strong>Q: Will the buyer view the tracking information after the order is fulfilled using EasyParcel plugin on WooCommerce?</strong></summary>

Yes, the customer can view it.

</details>

<details>
<summary><strong>Q: Conditions for WooCommerce orders to be imported</strong></summary>

**Requirements:**
- The order status is "processing" in woocommerce
- The order modified for the last 7 days
- The order not imported to Easyparcel before

**Reference path:**
- `portal-laravel/public/legacy/application/CUS_V8/Singapore/mvc/model/Database/cintegrationDB.php`
- `portal-laravel/public/legacy/application/CUS_V8/Malaysia/mvc/model/Database/cintegrationDB.php`

</details>

<details>
<summary><strong>Q: How to setup free shipping rules for EasyParcel rates on the checkout page? (guideline)</strong></summary>

The customer may add free shipping rule at the EasyParcel Courier Setting. Here are the steps:

1. Go to "WooCommerce" -> "Settings" -> "Shipping" -> "EasyParcel Courier Setting", click "Edit" on the zone that needs to add free shipping rule
2. Click "Edit" on the courier service added
3. Check the "Enable free shipping rule to apply" to enable free shipping rule, select "A minimum order amount" or "A minimum order quantity" at "Free shipping requires..", then value accordingly, then click "Save changes"

**Note:** Please note that the rates generated at the checkout page using our plugin currently does not support currency conversion, currently our plugin only supports Malaysia and Singapore rates. For example, if the Country selected at "EasyParcel Shipping" setting is "Malaysia" and the base currency of customer's woocommerce store is USD, the value of rates returned by our plugin will be in myr value but labelled as usd at the checkout page.

</details>

<details>
<summary><strong>Q: Why can't add courier on EP Courier setting tab</strong></summary>

Because User didn't set the shipping zone or didn't fill up the integration ID on EP setting page

</details>

<details>
<summary><strong>Q: Courier Setting > Locations not covered by your other zones</strong></summary>

Ask for their plugin version, older plugins will have this bug

</details>

<details>
<summary><strong>Q: Courier image not showing at checkout page</strong></summary>

If user using plugin version 1.0.7, the courier image will not show at checkout page is due to a bug.

If you're using version 1.6.8.18 or later and the courier image still isn't appearing, it could be because your chosen theme doesn't support the courier image. The default checkout theme does support it. To resolve this issue, you can either switch to a theme that supports the courier image or modify your current theme to enable it.

</details>

---

**Source Links:**
- Technical Questions: https://easyparcel.sg.larksuite.com/sync/Paidd7TbBs04xVbBWc9uYPBYsGc
- Operation Questions: https://easyparcel.sg.larksuite.com/sync/H6K9dPTULsLx4ObCZ81uZVzjsXd
