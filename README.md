![WhatsApp Image 2025-07-16 at 11 44 36_f8e66563](https://github.com/user-attachments/assets/a4e8a7c3-d072-490a-8734-0e775f493dfe)
![WhatsApp Image 2025-07-16 at 11 44 51_46ce4912](https://github.com/user-attachments/assets/e5c7019c-4865-42a3-9d74-8905afc82d95)
![WhatsApp Image 2025-07-16 at 11 45 30_e9658518](https://github.com/user-attachments/assets/9d174df5-39e4-4257-8b70-b3d94a3f91df)





# 🛍️ Twilio WhatsApp Retail Assistant Bot

A **multilingual, smart retail bot** built on **Twilio’s WhatsApp API** that helps manage inventory, take orders, show billing, and respond to customer queries in **English, Hindi, and Telugu**.

> 💬 Built for small businesses to operate seamlessly via WhatsApp — no app needed!

---

## 🌟 Features

- ✅ Add items to stock
- ✅ Book product orders
- ✅ Show running bill
- ✅ View available catalog
- ✅ See real-time stock
- ✅ Display offers and sales
- ✅ Multilingual responses (🇮🇳 Hindi, Telugu, English)

---

## 📱 How to Use via Twilio WhatsApp Sandbox

### 1️⃣ Create a Twilio Account
- Sign up: [twilio.com/try-twilio](https://www.twilio.com/try-twilio)
- Get your **Account SID** and **Auth Token**

---

### 2️⃣ Set Up WhatsApp Sandbox

- Visit: [console.twilio.com/sms/whatsapp/sandbox](https://console.twilio.com/sms/whatsapp/sandbox)
- Save:
  - **Sandbox number** (e.g., `+14155238886`)
  - **Join code** (e.g., `join brave-tiger`)

### 3️⃣ Join the Sandbox

Send your join code via WhatsApp to the sandbox number:

To: +14155238886
Message: join brave-tiger

yaml
Copy
Edit

---

### 4️⃣ Deploy Your Bot on Twilio Functions

- Go to: [console.twilio.com/functions](https://console.twilio.com/functions)
- Create a **new service** (e.g., `retail-bot`)
- Under the **Functions** tab:
  - Create a new function: `incoming.js`
  - Paste your bot logic (Node.js)
- Click **Deploy All**

> Don’t forget to update dynamic inventory/pricing if needed!

---

### 5️⃣ Connect Your Function to WhatsApp

In the WhatsApp sandbox settings, set:

WHEN A MESSAGE COMES IN: https://your-function.twil.io/incoming

yaml
Copy
Edit

✅ Done! You’re now ready to chat with your bot over WhatsApp.

---

## 🔤 Supported Languages

| Language | Detected Based On | Example Input |
|----------|-------------------|----------------|
| English  | Default fallback  | "Show stock" |
| Hindi 🇮🇳 | Devanagari (अ-ह) | "बिल दिखाएं" |
| Telugu 🇮🇳 | Telugu (అ-హ)     | "స్టాక్ చూపించు" |

---

## 💬 Sample Commands

| Intent         | English                 | Hindi                         | Telugu                      |
|----------------|-------------------------|-------------------------------|-----------------------------|
| Add Stock      | `add 5kg sugar`         | `5 किलो चीनी जोड़ें`          | `5 కిలోల చక్కెర జోడించు`      |
| Book Item      | `order 2kg rice`        | `2 किलो चावल बुक करो`         | `2 కిలో బియ్యం ఆర్డర్ చేయి`    |
| Show Bill      | `bill`                  | `बिल दिखाएं`                   | `బిల్ చూపించు`               |
| View Products  | `catalog` or `list`     | `उत्पाद`                       | `ఉత్పత్తులు`                  |
| Stock Check    | `stock`                 | `स्टॉक`                        | `స్టాక్`                      |
| Today's Offer  | `offer`                 | `ऑफर`                         | `ఆఫర్`                       |
| Help           | `help`                  | `मदद`                         | `సహాయం`                      |

---

## 📦 Example Flow

```text
👤: add 5kg sugar  
🤖: ✅ 5kg sugar added to inventory.

👤: order 2kg rice  
🤖: 📦 Order received: 2kg rice. ₹90 added to bill.

👤: bill  
🤖: 🧾 Your bill is ₹90.
