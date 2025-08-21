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
<summary><strong>Q:If after contacting Shopify support, the EasyParcel live rate still won't show in checkout page</strong></summary>

**A:** Kindly deactivate and activate the account page in the EasyParcel Shopify App.

<img width="1280" height="424" alt="image" src="https://github.com/user-attachments/assets/a1f18135-aa1a-48e8-b6ed-cda499a2aacb" />

</details>

<details>
<summary><strong>Q:Branch not available that I want to drop off</strong></summary>

**A:** You can drop off anywhere that the nearest branch near you,it won't affect anything on the shipping procedures as long as the parcel is scan into the courier system after drop off.

</details>

<details>
<summary><strong>Q:Fill in all correct detail in the order but the order wont appear in the app</strong></summary>

**A:** Check whether the order has a customer linked to it, as having a customer is required. Aadd a customer to the order so it can be viewed in the EasyParcel Shopify App.

Example error photo:
<img width="1280" height="175" alt="image" src="https://github.com/user-attachments/assets/619f68af-dba4-4023-89d9-1fc5904f3c40" />

</details>

<details>
<summary><strong>Q:What if the settings in Shopify and EasyParcel App are correct but the live rate still not displaying at the checkout page</strong></summary>

**A:** The courier option may not support the selected delivery location, which is why it does not appear on the checkout page.

</details>

<details>
<summary><strong>Q: Will orders imported automatically when customer placed orders (Import Version)?</strong></summary>

**A:** Yes, the order will import automatically if the auto import settings is turn on. But the order may not immediately imported once customer placed as our auto import settings, will only be triggered a few times a day.

</details>

---

**Source Links:**
- Technical Questions: https://easyparcel.sg.larksuite.com/sync/Paidd7TbBs04xVbBWc9uYPBYsGc
- Operation Questions: https://easyparcel.sg.larksuite.com/sync/H6K9dPTULsLx4ObCZ81uZVzjsXd
