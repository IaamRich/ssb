# SMSSpamBlocker 📵✉️

**SMSSpamBlocker** is a cross-platform mobile application built with **.NET MAUI** that automatically detects and removes unwanted spam SMS messages.  
It ensures that spam senders (e.g., "SomeOnlineShop") are blocked silently: notifications briefly appear but are immediately dismissed once the message is filtered and removed.

---

## 🚀 Features

- 📩 **Real-Time SMS Monitoring** – Track all incoming SMS messages as soon as they arrive.  
- 🛑 **Automatic Spam Removal** – If the sender matches the user’s blacklist, the SMS is deleted and the notification disappears.  
- 📋 **Custom Blacklist** – Add sender names or numbers to your personal spam list.  
- 🔔 **Silent Filtering** – Spam notifications vanish right after they appear.  
- 📊 **History Log** – View blocked/deleted SMS attempts for audit.  
- ⚙️ **Cross-Platform Targeting** – Android and iOS supported.

---

## 🧑‍💻 Tech Stack

- **.NET MAUI** – Cross-platform framework for building native apps.  
- **C# 12** – Business logic and services.  
- **XAML** – UI layouts.  
- **Platform APIs** – Native integration for SMS interception and notification handling.  

---

## 📱 Platforms

### ✅ Android
- Full support for SMS interception and removal.  
- Works by registering the app as the **default SMS handler**.  
- When a spam SMS arrives:
  1. System notification appears.  
  2. App checks sender name/number.  
  3. If in blacklist → SMS deleted, notification cleared instantly.  

### ⚠️ iOS
- On **iOS** → messages go to **Junk**, notification auto-disappears, but SMS stays. 
