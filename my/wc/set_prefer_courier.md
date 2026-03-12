# Set Prefer Courier Option 🚚 display to your customer in your Woocommerce Store.
This guideline is help you to set the courier 🚚 that you prefer to display in the customer checkout page.


## Navigation path
**Woocommerce -> Settings -> Shipping** -> **Shipping zones**
### Shipping Zones Settings
press the **Add Zones** button

<img width="609" height="355" alt="Screenshot 2026-02-27 at 4 05 10 PM" src="https://github.com/user-attachments/assets/818402c0-3f6e-4728-984d-13cfd5db50b5" />

The diagram above shows the WooCommerce Shipping Zones settings. This configuration allows store owners to define default shipping rules based on regions. Merchants can specify which regions they want to serve and assign the available shipping methods for each region. When a customer enters a shipping address that falls within a defined region, WooCommerce will automatically apply the corresponding shipping methods.

---

1. Enter the Zone Name
2. Select the Region that include in the Zone
3. Press the **Add Shipping method** button
<img width="1120" height="557" alt="Screenshot 2026-02-27 at 4 20 24 PM" src="https://github.com/user-attachments/assets/71b2ea26-0f98-4d22-b80c-0b9faa7a3e26" />

Choose the **EasyParcel Shipping** -> Press Continue
<img width="1119" height="621" alt="Screenshot 2026-02-27 at 4 20 35 PM" src="https://github.com/user-attachments/assets/a2e3e03c-1e68-4268-a7a6-7fbeab6abe51" />

Make Sure that the EasyParcel Shiping is in the Shipping methods.
<img width="840" height="204" alt="Screenshot 2026-02-27 at 4 21 12 PM" src="https://github.com/user-attachments/assets/2ebfda42-182d-42e1-b31b-c994ed0eaa28" />

If yes, press the **save changes** button, and you may proceed to EasyParcel Courier Settings.

### **EasyParcel Courier Settings**
<img width="669" height="394" alt="Screenshot 2026-02-27 at 4 04 53 PM" src="https://github.com/user-attachments/assets/f489cc6f-5171-47ce-af40-66c9cf7ed3b8" />

this page shows the EasyParcel courier settings in WooCommerce. These settings are used to automatically determine which courier services are available and displayed on the checkout page.

---
1. Enter the Zones Name
2. Select the Destination (Zone Regions in Shipping Zones Settings)
3. Press the **Add courier service** button
<img width="1120" height="557" alt="Screenshot 2026-02-27 at 4 34 54 PM" src="https://github.com/user-attachments/assets/c789b59d-00a1-49ff-b015-94a4eb6cb3ae" />

Select the courier that you prefer to show in the check-out page. You may also change the courier name in the **Courier Display Name** Text Box.
<img width="1100" height="429" alt="Screenshot 2026-02-27 at 4 35 47 PM" src="https://github.com/user-attachments/assets/5a5ba444-951a-46a4-988d-9b835614a853" />

You may enable the free shipping rule (optional)
<img width="1120" height="206" alt="Screenshot 2026-02-27 at 4 35 56 PM" src="https://github.com/user-attachments/assets/d3b7d51b-eecf-415a-9b41-0c70733f4405" />

🚨 System flow explanation
1. The system first checks the customer’s shipping address and matches it with the configured Shipping Zones in WooCommerce to determine the applicable shipping method.
2. If the shipping method for that zone is set to EasyParcel Shipping , the system will then refer to the EasyParcel courier settings . Based on the customer’s region, it will retrieve and display the available couriers and default courier options from EasyParcel.
