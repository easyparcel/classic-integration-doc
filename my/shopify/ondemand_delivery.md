# On-Demand Delivery — Shopify

On-Demand delivery lets you send a Shopify order **point-to-point** with an instant courier (e.g. **Grab**, **Lalamove**) instead of a standard parcel service. You set a pick-up and drop-off location on a map, get live quotes, pick a courier, and the driver collects and delivers on the schedule you choose.

> ℹ️ On-Demand is available when your **sender (pick-up) address is in Malaysia (MY) or Singapore (SG)**.

---

## Table of contents

1. [Fulfil a single order with On-Demand](#3-fulfil-a-single-order-with-on-demand)
2. [Bulk On-Demand booking](#4-bulk-on-demand-booking)
3. [Track & manage an On-Demand order](#5-track--manage-an-on-demand-order)
4. [Tips & troubleshooting](#6-tips--troubleshooting)

---

## 1. Fulfil a single order with On-Demand

### Step 1 — Open the order and choose On-Demand

Open an unfulfilled order in the EasyParcel app. When On-Demand is available you'll see two tabs at the top of the fulfilment card:

- **Standard delivery**
- **On-Demand delivery**

Click **On-Demand delivery**.

<img width="100%" alt="Screenshot 2026-07-31 at 5 52 02 PM" src="https://github.com/user-attachments/assets/de48da3c-5565-4f8a-b9a0-d7a35bb28426" />


> 🔒 While an order is being placed, the tabs are **locked** so you can't switch modes mid-booking.

### Step 2 — Set the Pick Up and Drop Off point

The **Pick Up** section is pre-filled from your selected sender address. The **Drop Off** section is pre-filled from the order's shipping address.

- Search / drag the pin / paste a coordinate to fine-tune the exact collection spot.
- Add **pick-up remark** and **drop-off remark** for the driver.
- Confirm the pin location — **drag it to the exact door** if the geocoded spot is off.

<img width="100%" alt="Screenshot 2026-07-31 at 5 54 40 PM" src="https://github.com/user-attachments/assets/8a129b1b-e5d2-45fa-bfc4-277c98171a2b" />

### Step 3 — Enter parcel details

Fill in each parcel:

- **Content** (item description)
- **Quantity**
- **Weight (kg)**
- **Length / Width / Height (cm)**

> ⚠️ **Weight and each dimension must be at least `0.1`.** Empty, zero or negative values are rejected.

Use **Add parcel** for multiple items in one booking. The combined size shown is what to match against the vehicle you pick.

<img width="100%"  alt="Screenshot 2026-07-31 at 6 07 27 PM" src="https://github.com/user-attachments/assets/33259c55-865b-4bc1-a639-b1be90e9bc59" />


### Step 4 — Set the schedule

Choose the **pick-up date** and **pick-up time**.

- You can't schedule a **date/time in the past**.
- If you keep **today's date**, the time can't be earlier than now.

<img width="100%"  alt="Screenshot 2026-07-31 at 6 09 42 PM" src="https://github.com/user-attachments/assets/7fd08c4d-55ec-45d5-9197-fb4291f13918" />



### Step 5 — Get a quotation and choose a courier

Click **Get quotation** (or **Refresh rates**). Available couriers and their prices appear (e.g. Grab, Lalamove). Select the one you want.

> If you change the schedule or move a pin, the old quote clears and re-quotes automatically.

<img width="100%" alt="629636856-6374ddc0-0d95-4fd7-8c8a-8bcb1610e2b2" src="https://github.com/user-attachments/assets/90e7e800-8f0a-4ce1-b429-1b4979a43472" />


### Step 7 — Place the order

Click **Place on-demand order**. The amount is charged to your credit, the booking is created, and the driver is dispatched per your schedule.

<img width="100%"  alt="Screenshot 2026-07-31 at 6 12 53 PM" src="https://github.com/user-attachments/assets/e00eafca-5c33-445e-b56e-0317aa57f2d4" />

---

## 2. Bulk On-Demand booking

To book several orders at once:

1. Go to the **Orders** list in the app. Select the orders you want to send. Choose the **On-Demand** bulk action to open the bulk composer.
   <img width="100%" alt="Screenshot 2026-07-31 at 6 16 13 PM" src="https://github.com/user-attachments/assets/ed4bcb6f-94e5-419c-92d7-88e2151efa67" />


2. The bulk on-demand booking page has two sections:

   **Pickup Details**: the card on the top show the pickup details including sender address chosen, pickup location coordinate, sender details (phone number/email) and scheduled pickup date/time

   **Booking List**: the section below list all bookings in this bulk.
   > By default, the order that having same shipping address will be auto merge into same dropoff point.
   > You may also select one or more bookings to group into single booking.
   > The page pre-quotes and pre-selects the cheapest courier where possible.
   <img width="100%" alt="Screenshot 2026-08-03 at 4 01 14 PM" src="https://github.com/user-attachments/assets/428bddb3-8a15-4da3-bc3d-0440e6c229c6" />

   - For each booking, you may click **Edit details** button to edit the booking details including pickup remark, dropoff point location and parcels, and courier service selected

3. Finally, review the total and **place** all bookings.


---

## 3. Track & manage an On-Demand order

Once placed, the order shows its On-Demand booking details:

- **Booking status** (Pending → Accepted → In Transit → Fulfilled, etc.)
- **Tracking link**
- **Driver details** once assigned
- **Cancel booking** (only while the booking is still cancellable, e.g. pending / no driver found)

<img width="100%" alt="image" src="https://github.com/user-attachments/assets/16475862-6228-4c80-a069-c17ccb9230bf" />


**Cancelling:** if a booking is still cancellable, use **Cancel booking**. On a successful cancel the charge is refunded to your credit.

---

## 4. Tips & troubleshooting

### Address can't be found

If searching an address returns no result, the panel shows a fallback message with:

- a **"Find this address on Google Maps"** link, and
- a hint to **copy the coordinates** (e.g. `3.1390, 101.6869`) and **paste them back** into the search box.

Paste the coordinate and press **Search** — the pin drops exactly there.



> The address search also understands common Malaysian short-forms (e.g. **`jln` → `jalan`**) and automatically retries with a simpler version of the address, so a slightly-off address usually still resolves.

### The pin is in the wrong place

Search, **click the map**, or **drag the pin** to correct it. The pinned spot is approximate — always confirm the exact door before booking.

### "Weight/dimension must be at least 0.1"

Every parcel needs a **weight and length / width / height of at least `0.1`**. Fix the highlighted field and try again.

### The tabs are greyed out

That's expected **while an order is being placed** — switching is disabled until the booking finishes.
