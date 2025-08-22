# EasyParcel API FAQ

<details>
<summary><strong>Minimum Order Quantity (MOQ)</strong></summary>

### Q: What is MOQ (Minimum Order Quantity) pick up by courier services?

`require_min_order` is set as 0 because the parcel could be accumulated, as long as the parcel is more than 3, the relative courier service will go and pick up the parcels.

If you wishes to filter up the courier services that is having MOQ, you may to filter by searching the key words of "Pick Up with min" as some of the MOQ of courier services are different. Hence, the suggestion is only filter with the key words of "Pick Up with min".

</details>

<details>
<summary><strong>Courier Services</strong></summary>

### Q: How can I fix the certain couriers?

**May refer to all of the courier from list below:**

Individual API documentation > Rate Checking > "service_id" result.

**Reference link:** https://developers.easyparcel.com/#nav_Individual_EPRateCheckingBulk

The sorting or filtering the list to user's platform is allowable. However, EasyParcel is not providing the technique currently.

If to call for courier partners' estimated delivery days, may refer to the result from:
Individual API documentation > Rate Checking > "delivery" result

### Q: May I get the list of couriers supported by easyparcel?

**Current courier list with id (22th Aug 2025):**

- EP-CR0AX - Aramex International Logistics Pte Ltd
- EP-CR0AS - SF Express (Singapore) Pte Ltd.
- EP-CR0AK - United Parcel Service Singapore Pte Ltd
- EP-CR0AC - XDel Singapore Pte Ltd
- EP-CR0A3 - Airpak Express Pte Ltd
- EP-CR0AO - Park N Parcel Pte Ltd
- EP-CR0AV - Ninja Logistics Pte.Ltd
- EP-CR0A8 - Janio Technologies Pte Ltd
- EP-CR0DA - J&T Express Singapore Pte Ltd
- EP-CR0DD - Singapore Post Limited
- EP-CR0DF - TracX Logis Pte. Ltd
- EP-CR0DG - Pickupp Pte Ltd
- EP-CR0DY - TNT Express Worldwide (S) Pte Ltd
- EP-CR0DB - Federal Express (Singapore) Pte. Ltd
- EP-CR0DJ - Teleport Everywhere Pte Ltd
- EP-CR0DZ - MXHL Pte Ltd
- EP-CR0D2 - City-Link Express & Logistics (S) Pte Ltd
- EP-CR0IF - SPX Express Private Limited


### Q: Why FedEx and UPS will not return on External API?

 UPS and Fedex will be not available in all integration system including Woocommerce plugin, shopify app, easystore and API. While For Shopify and woocommerce import is still available.
  Our engineering team are not planning to implement both courier in our integration system anytime soon, as due to some technical issue, the implementation will cause our api to have slow respond time.

</details>

<details>
<summary><strong>Email and Order Functions</strong></summary>

### Q: Able to advise on this, as customer asks if he can input the receiver's email for API Call for the function EPSubmitOrderBulk?

- The EPSubmitOrderBulk function does not include the email sending feature and the email only sends to the sender after done the EPPayOrderBulk function.
- If the sender wants to send email to the receiver after done EPPayOrderBulk function, the sender can go to EasyParcel -> Marketing tools -> Custom Branding -> Tracking Email to setup the email content.
- Once EPPayOrderBulk is done, we will send the email to the receiver according to email that setup by the sender.

</details>

<details>
<summary><strong>Demo and Testing</strong></summary>

### Q: Demo environment respond time

This was due to our server spec being low, that's why it will take longer respond time.

</details>

<details>
<summary><strong>Error Handling</strong></summary>

### Q: Submit order API get error: Invalid Zipcode...

- Check if postcode is valid
- Postcode should not have dash

### Q: Why does EPOrderStatusBulk API call still return 'Order does not exist' after the order is successfully submitted in DEMO environment?

This issue should only happen in DEMO environment because the order submitted is not inserted into the database.

**Note:** Even in LIVE environment, if the order status checking API is called right after the order is submitted, you may also get the 'Order does not exist' message due to the delay. In this case, you may try again to get the order status later, maybe after 5 minutes.

### Q: If the AWB is null in response to pay order API call

**In live environment:** Please call the pay order API again on the same order_number. This usually happens due to our API failing to retrieve the AWB from courier during the payment. Calling pay order API on the same order won't charge twice.


### Q: If API shows invalid on Postman

**Reason 1:** This might be due to us updating our service id at that time.

**Reason 2:** It might be due to customer using live environment to submit order and use demo environment for rate checking. Our demo and live environment are different that's why when user calls it will show invalid.

### Q: Rate checking on Postman if takes long time

It may be due to our server experiencing high load at that time that's why it will slow down the response time.

</details>

<details>
<summary><strong>API Features and Limitations</strong></summary>

### Q: Can I filter the courier companies to be returned from the API response by passing parameter "exclude_fields"?

No. Currently, our API does not provide the feature of filtering courier company to be returned.

### Q: How many items can a customer fulfill in 1 single bulk request?

Up to 300 per bulk request.

### Q: Is it possible to use two types of API together (Individual and marketplace)?

It is possible to use two types of API key together.

</details>

<details>
<summary><strong>Pricing and Differences</strong></summary>

### Q: Why is there a difference in price between portal and API?

The price customer gets during quoting is not the final price yet. They may proceed with booking and checkout, then they will be able to see the shipment tax and add-on service charges if applied. The prices between EasyParcel portal and API are the same.


**Full explanation:**
It is due to not all our partners being fully integrated with our system, which updates from time to time. Therefore, we provide standard higher prices, including add-on charges, during quotations to our partners to avoid undercharges. Thus, there will be a 0.20 price difference as a result, the quotations may be higher than the actual payment prices.


</details>

<details>
<summary><strong>COD and Special Services</strong></summary>

### Q: Cannot get COD - "cod_service_available": "false"

Their width, length and height are too small, like 0.1cm x 0.1cm x 0.1cm. Ask them to put at least 1 x 1 x 1 and make sure they know what weight dispute is.

</details>

<details>
<summary><strong>Collection and Delivery</strong></summary>

### Q: Do Hong Kong postcode required in API call
 No
### Q: Will Order submitted to EasyParcel will be expired if the coll_date is passed by the order not paid yet?
 Yes


### Q: The maximum collect_date can be specified in External API is only 14 days from the date calling the API

This is maximum. Some couriers only support the coll_date to be specified 7 days from the day calling the API.

### Q: API Response msg: "Kindly change the chosen pickup date or choose another courier service"

The coll_date they input is invalid (for example, 2 days before the current day). External API will reorder year-month-day then pass to legacy internal API but will not choose a valid date (job for internal API) and problem should be bug in internal API.

**Sample response:**
After checking, we noticed you passed the coll_date is 2025-01-06. While we are able to auto assign coll_date to the next day if it is not valid, we recommend submitting the current date, or if you wish to schedule the order later kindly pass a future date.

</details>

<details>
<summary><strong>Notifications and Tracking</strong></summary>

### Q: Email, SMS, WhatsApp tracking. When will the buyer start to get the notification?

When the courier confirms that the parcel is with them, it will start to notify the customer through webhook until the parcel is received by the buyer.

</details>

<details>
<summary><strong>Regional Specific</strong></summary>

### Q: SG merchant fulfill using dropoff courier service, portal shows it as pickup

External API does not provide dropoff points for all SG courier services in rate checking, so customer have no choice but to submit without dropoff points. Dropoff orders submitted without dropoff point will become pickup orders.

However portal provides option to pick dropoff point so you may ask them to fulfill there. The integration team does not have any plans to fix the issue for legacy external API.

### Q: Does Singapore have shipping tax?

Please note that Singapore does not impose shipping tax, even for international shipments. However, Malaysia does apply shipping tax, commonly referred to as SST (Sales and Services Tax).

</details>

<details>
<summary><strong>Portal Related Issue</strong></summary>

### Q: Why the failed order submitted from API will auto add to cart on portal?

It's not an auto add to your cart, but the portal will alert you that you have unpaid order and will move your unpaid order back to your cart.

If you ignore the alert (where you didn't click the button "Bring Me to My Cart", or click the alert box from the top right alert box), then the item will not be added back to your cart. This is part of our portal user experience where if the user clicks checkout, and they do not complete the payment, then the alert will be triggered 5 minutes later.

From API side, because your request submitted to our system, but the payment fails, therefore the system treats this as an unpaid order and it will notify from the portal as normal activities.

### Q: If customer asks why the courier name during submit order and rate checking courier name is slightly different for MPRateChecking and MPSubmitOrder

The full courier name during rate checking is the full courier name while, the courier name shown after submit order are the courier short name.

*May provide reference file for them to refer.*

</details>
