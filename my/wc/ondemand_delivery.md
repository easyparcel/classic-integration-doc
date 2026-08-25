# On-Demand Delivery — WooCommerce

On-Demand delivery lets you send a WooCommerce order **point-to-point** with an instant courier (e.g. **Grab**, **Lalamove**) instead of a standard parcel service. You set a pick-up and drop-off location on a map, get live quotes, pick a courier, and the driver collects and delivers on the schedule you choose.

> ℹ️ On-Demand is available when your **sender (pick-up) address is in Malaysia (MY) or Singapore (SG)**.

> 🖼️ **Note for maintainers:** the `![...](images/...)` lines below are placeholders. Replace each image, or capture the screenshot described in the `<!-- 📸 ... -->` comment above it. Put images under `docs/images/woocommerce/`.

---

## Table of contents

1. [Before you start](#1-before-you-start)
2. [Set your pick-up (sender) address](#2-set-your-pick-up-sender-address)
3. [Fulfil a single order with On-Demand](#3-fulfil-a-single-order-with-on-demand)
4. [Bulk On-Demand booking](#4-bulk-on-demand-booking)
5. [Let buyers pin their location at checkout (optional)](#5-let-buyers-pin-their-location-at-checkout-optional)
6. [On-Demand live rate at checkout (optional)](#6-ondemand-shipping-price-at-checkout-optional)
7. [Track & manage an On-Demand order](#6-track--manage-an-on-demand-order)
8. [Tips & troubleshooting](#7-tips--troubleshooting)

---

## 1. Before you start

You'll need:

- The **EasyParcel Shipping** plugin installed, activated and connected (Integration ID set).
- Enough **EasyParcel credit** — On-Demand bookings are charged to your credit when you place the order.
- A **sender address in MY or SG** (see the next section).
- An order that is **not yet fulfilled**.

---

## 2. Set your pick-up (sender) address

Your pick-up location comes from your **sender address**. An accurate map pin here means the courier collects from the right spot.

1. Go to **WooCommerce → Settings → Shipping → EasyParcel**.
2. Open / add a **Sender Address** and fill in the address fields.
3. Use the **map** to set the exact pick-up spot:
   - Type in the **Search address** box and press **Search**, then pick a suggestion, **or**
   - **Click** the map / **drag the pin**, **or**
   - Paste a **coordinate** (e.g. `3.1390, 101.6869`) into the search box and press **Search** — the pin drops straight to it.
4. **Save**. The coordinate is stored and reused as your On-Demand pick-up point.
   <img alt="01-sender-address-map" src="https://github.com/user-attachments/assets/1c3ed289-1800-45bc-aebf-ece141b35f20" />


> 💡 If the address can't be found, see [Address not found](#address-cant-be-found) below.

---

## 3. Fulfil a single order with On-Demand

### Step 1 — Open the order and choose On-Demand

Open an unfulfilled order in **WooCommerce → Orders**. In the **EasyParcel** fulfilment box you'll see two tabs:

- **Standard**
- **On-Demand**

Click **On-Demand**.

<img  alt="02-tabs" src="https://github.com/user-attachments/assets/bc031029-9fe7-4867-97eb-210d8144ada0" />


> 🔒 While an order is being placed (Standard **or** On-Demand), the tabs are **locked** so you can't switch modes mid-booking.

### Step 2 — Set the Pick Up point

The **Pick Up** map is pre-filled from your selected sender address.

- Search / drag the pin / paste a coordinate to fine-tune the collection spot.
- Switching the **sender address** dropdown updates the pick-up location automatically.
- Add a **pick-up remark** for the driver if needed.
  <img  alt="03-pickup" src="https://github.com/user-attachments/assets/bbb70ffe-d26e-43ac-9330-15211a1541fa" />

### Step 3 — Set the Drop Off point

The **Drop Off** map is pre-filled from the order's shipping address.

- Confirm the pin — **drag it to the exact door** if the geocoded spot is off.
- Add a **drop-off remark** (required) — this is what the driver sees.
  <img  alt="04-dropoff" src="https://github.com/user-attachments/assets/0e02f5fc-1a18-424b-8bc9-8a0092a4b79f" />


### Step 4 — Set the schedule

Choose the **pick-up date** and **pick-up time**.

- You can't schedule a **date/time in the past**.
- If you keep **today's date**, the time can't be earlier than now.
  <img alt="05-schedule" src="https://github.com/user-attachments/assets/a8a0607f-e0a8-4ef4-8a6f-6621192e896c" />


### Step 5 — Enter parcel details

Fill in each parcel:

- **Description** (item content)
- **Qty**
- **Weight (kg)**
- **Length / Width / Height (cm)**

> ⚠️ **Weight and each dimension must be at least `0.1`.** The modal won't close and the order can't be placed until every parcel is valid — invalid fields are highlighted in red.

Use **Add parcel** for multiple items in one booking.
<img alt="06-parcels" src="https://github.com/user-attachments/assets/ea36dcb3-a0e7-4bfb-85d1-41b6eb0b8f66" />


### Step 6 — Get a quotation and choose a courier

Click **Get quotation** (or **Refresh rates**). Available couriers and prices appear (e.g. Grab, Lalamove). Select the one you want.

> Changing the schedule or moving a pin clears the quote and re-quotes automatically.

<img alt="07-quotes" src="https://github.com/user-attachments/assets/41b228cb-4ed5-487b-ba26-f438dec88a11" />


### Step 7 — Place the order

Click **Place on-demand order**. The amount is charged to your credit, the booking is created, and the driver is dispatched per your schedule.

<img  alt="08-place-order" src="https://github.com/user-attachments/assets/b8cf2eb2-b53e-4e08-bf56-b5f9abcfe8ed" />

---

## 4. Bulk On-Demand booking

To book several orders at once:

1. Go to **WooCommerce → Orders**.
2. Select the orders, then choose the **On-Demand bulk fulfil** action.
3. In the composer, orders sharing the **same shipping address are auto-merged** into one drop-off point.
4. For each booking, pin the drop-off(s), fill parcel details, set the schedule and pick a courier.
5. Review the total and **place** all bookings.
   <img alt="09-bulk" src="https://github.com/user-attachments/assets/48aa53bc-a603-4007-bd4a-ee442f276950" />

---

## 5. Let buyers pin their location at checkout (optional)
### Add map pin in checkout page
Enable the **Buyer Location Pin at Checkout** at **EasyParcel Shipping** setting to add a address search field and map picker at the checkout page
<img alt="" src="https://github.com/user-attachments/assets/6b572d3e-bce7-43a7-a75a-5f1ae59db0da" />

Once enabled, buyers choosing an On-Demand method at checkout can **search and pin their exact delivery location** on a map. That pinned coordinate is then used as the drop-off when you fulfil the order — no need to correct the pin later.

<img alt="10-checkout-pin" src="https://github.com/user-attachments/assets/18886a60-0424-48b9-b289-6898db4b66a5" />


---

## 6. On-Demand live rate at checkout (optional)
This setting allow you to add EasyParcel ondemand courier service as shipping method at the checkout page. The shipping price will calculated based on the location of your default sender address and the buyer pin location.

### Steps to set ondemand checkout shipping price
1. Click **Add shipping method** on the shipping zone
   <img  alt="" src="https://github.com/user-attachments/assets/f72ebb27-0f22-4dc1-a0b0-b6112eab746b" />

3. Select **EasyParcel On-Demand** option
   <img alt="" src="https://github.com/user-attachments/assets/1c44c642-7f61-4ee7-8c01-27c921cd6f81" />

5. Click **Edit** button to set the type of the shipping price
   <img  alt="" src="https://github.com/user-attachments/assets/4757c80f-2513-46ef-9302-f4415ba3a022" />

7. Choose the options based on the need:
   <img  alt="" src="https://github.com/user-attachments/assets/3ff0b6ad-30be-430c-9b6a-5382c6e21ab8" />
   - **All on-demand couriers**: display all available courier service for the given route
     <img alt="" src="https://github.com/user-attachments/assets/d500061c-fa4a-457a-964a-1e53a257bb74" />

   - **Cheapest on-demand courier**: display cheapest courier service for given route
     > "Auto-select one option based on cart weight" option will select one cheapest service based on cart item weight
     <img alt="" src="https://github.com/user-attachments/assets/0ee222d6-9369-4f73-934b-a9705c333ec9" />

   - **Specific courier (s)**: display specific courier only for given route
     
       **By courier**: Only show specific courier (Lalamove, Pandago, etc) 
       <img alt="" src="https://github.com/user-attachments/assets/2966c8d3-401c-43f0-8a02-88cb6dd6c6cc" />
       **By service**: Only show specific courier service (Lalamove car, Lalamove bike, etc)
       <img alt="" src="https://github.com/user-attachments/assets/222882ff-bec3-4d74-9e40-5c11dffb984a" />


---

## 7. Track & manage an On-Demand order

After placing, the order's fulfilment box shows the On-Demand booking:

- **Booking status** (Pending → Accepted → In Transit → Fulfilled, etc.)
- **Tracking link**
- **Driver details** once assigned
- **Cancel booking** (only while still cancellable, e.g. pending / no driver found)
  <img alt="11-fulfilled" src="https://github.com/user-attachments/assets/ffd35004-8e31-4816-ac42-d98d0ca01338" />


**Cancelling:** if a booking is still cancellable, use **Cancel booking**. On a successful cancel the charge is refunded to your credit.

---

## 8. Tips & troubleshooting

### Address can't be found

If searching an address returns no result, the map shows a fallback with:

- a **"Find this address on Google Maps"** link, and
- a hint to **copy the coordinates** (e.g. `3.1390, 101.6869`) and **paste them back** into the search box.

Paste the coordinate and press **Search** — the pin drops exactly there.
<img alt="12-not-found" src="https://github.com/user-attachments/assets/7aff9d62-395c-4114-be4c-be3b13fb06c0" />


> The search also understands common Malaysian short-forms (e.g. **`jln` → `jalan`**) and automatically retries with a simpler version of the address, so a slightly-off address usually still resolves.

### The pin is in the wrong place

Search, **click the map**, or **drag the pin** to correct it. The pinned spot is approximate — always confirm the exact door before booking.

### "Weight/dimension must be at least 0.1"

Every parcel needs a **weight and length / width / height of at least `0.1`**. Fix the highlighted field(s) — the modal won't close until all parcels are valid.

### The tabs are greyed out

That's expected **while an order is being placed** — switching is disabled until the booking finishes.
