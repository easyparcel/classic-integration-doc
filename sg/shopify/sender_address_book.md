# Introduction: Sender Address Book

The EasyParcel Shopify App provides a **Sender Address Book** feature that allows merchants to create and manage multiple sender addresses within the app.

With this feature, merchants can:
- Add and store multiple sender addresses (e.g. warehouse, office, or branch locations)
- Easily select a preferred sender address during the order fulfillment process
- Update or remove sender addresses as business needs change

This improves fulfillment accuracy and flexibility, especially for merchants managing shipments from multiple locations.

## Sender Address Setting
1. In the Shopify, open **EasyParcel- Delivery Made Easy** app, go to **Setting > Shipping Setting**, ensure you have already verified the integration id by clicking **Verify** button.

   <img width="1203" height="619" alt="Screenshot 2026-01-08 at 1 35 30 PM" src="https://github.com/user-attachments/assets/58dba00f-c6af-49fa-9559-1bc448b11b82" />


2. Scroll down to the sender details section.

   <img width="100%" height="535" alt="Screenshot 2026-01-08 at 1 44 24 PM" src="https://github.com/user-attachments/assets/38558d2d-9c56-4661-8cfe-ce88e66b673e" />

   Here, the user can fill in the sender details and manage their sender addresses.
   
   * **Custom Locations**: Sender Addressess that user manually add.
     * **+ Add Location** button: Click to add a new sender address. A form will be shown after clicked to fill in the address details. Fill in the address details and click **Save** button to save the new address.
       
       <img width="671" height="595" alt="Screenshot 2026-01-09 at 9 48 52 AM" src="https://github.com/user-attachments/assets/05c75e3c-e10b-4e20-9feb-f745c3510a39" />

     * **Load EasyParcel Profile Address** button: Click to fetch profile address of EasyParcel account. The sender details above (email, company name, name and phone number) will also be loaded if it is not filled in yet

   * **Shopify Locations**: Sender Addresses that fetched from user's store locations.
     * **Load Location** button: Click to fetch the user's store location

3. Once successfully adding or loading the address, it will display immediately in each section and each address will have several action buttons to use

   <img width="767" height="423" alt="Screenshot 2026-01-09 at 9 57 52 AM" src="https://github.com/user-attachments/assets/6a9212da-050a-41b8-94d9-c7060e1877f2" />

   * **Set as Default** button: To make the address as default address. Default address will be
     
     > - Used during auto fulfillment
     > - Pre-selected in order fulfillment page
     > - Used to calculate checkout live rates
   
   * **Edit icon** button: To edit the details of the address, a form will be shown to edit the details. Edit and click **Save** button to make the changes take effect.
   * **Delete icon** button: To delete the address. Once it is deleted, it can't be restored back, so be careful on the delete action


## Sender Address Selection: Single Fulfillment
1. In order fulfillment page, there will be a **Sender Address** section that displays what sender address will be used in fulfillment. The user can click **Change Sender Address** button to perform several actions such as choose another address, add new address or edit existing address.
    
   <img width="100%" alt="Screenshot 2026-01-09 at 11 43 34 AM" src="https://github.com/user-attachments/assets/0ddb18da-b8bd-45e4-961e-d49941fe2937" />
2. Once **Change Sender Address** button is clicked, a address selection form will be displayed.
   
   <img width="100%" alt="Screenshot 2026-01-09 at 11 47 41 AM" src="https://github.com/user-attachments/assets/0adb2727-1b5e-4917-b661-f7698a551771" />

   * **+ Add Address** button: To add a new custom address. A form will displayed allowing user to fill in address details. Fill in the address details and click **Save** button to save the new address.
     
     <img width="100%" alt="Screenshot 2026-01-09 at 11 52 33 AM" src="https://github.com/user-attachments/assets/5c1993ec-efa5-411e-ac38-f9bab3286dd1" />
   * **Edit icon button**: To edit a specific address. A form will be shown to edit the details. Edit and click **Save** button to make the changes take effect.
   * **Close** button: To close the address selection form.

4. Once the address selection form is closed, the selected address will be used.

## Sender Address Selection: Bulk Fulfillment
1. In order fulfillment page, there will be a **Sender Address** section that displays what sender address will be used in fulfillment. The user can click **Change Sender Address** button to perform several actions such as choose another address, add new address or edit existing address.
   <img width="100%" alt="Screenshot 2026-01-09 at 12 03 53 PM" src="https://github.com/user-attachments/assets/e96671d2-e186-4b44-8c73-4b44c105e9ff" />

   
2. Once **Change Sender Address** button is clicked, a address selection form will be displayed.
   
   <img width="100%" alt="Screenshot 2026-01-09 at 11 47 41 AM" src="https://github.com/user-attachments/assets/0adb2727-1b5e-4917-b661-f7698a551771" />

   * **+ Add Address** button: To add a new custom address. A form will displayed allowing user to fill in address details. Fill in the address details and click **Save** button to save the new address.
     
     <img width="100%" alt="Screenshot 2026-01-09 at 11 52 33 AM" src="https://github.com/user-attachments/assets/5c1993ec-efa5-411e-ac38-f9bab3286dd1" />
   * **Edit icon button**: To edit a specific address. A form will be shown to edit the details. Edit and click **Save** button to make the changes take effect.
   * **Close** button: To close the address selection form.

4. Once the address selection form is closed, the selected address will be used.
