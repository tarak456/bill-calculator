# bill-calculator
A simple web-based kirana store bill clculator using html,css and javascript.
# 🛒 Kirana Store Bill Calculator

A simple **web-based billing system** for small Kirana shops, made using **HTML, CSS, and JavaScript**.  
It allows shopkeepers to add purchased items with quantity and price, automatically calculates totals, and shows an updated bill list.

---

## 📌 Features
- Add items with name, quantity, and price.
- Automatically calculates **total price** for each item and adds it to the bill.
- Displays an **ongoing bill list** with all previously added items.
- Updates **total amount** without refreshing the page.
- Stylish and responsive design using **CSS**.

---

## 🛠️ Technology Used
- **HTML** → Structure of the calculator.
- **CSS** → Styling, colors, and layout.
- **JavaScript** → Bill calculation logic and dynamic updates.

---

## 🔍 How the Script Works
1. **User Input** → Item name, quantity, and price are entered in input fields.
2. **JavaScript Processing**:
    - Calculates total for that item:  
      ```javascript
      let total = quantity * price;
      ```
    - Adds it to the **existing total amount** in memory:  
      ```javascript
      totalAmount += total;
      ```
    - Creates a new `<li>` in the bill list to display the item details.
3. **Bill List Updates** → Older items remain because each new item is appended instead of replacing previous ones.

---

## 📦 Storage & Processing Logic
- No **database** or **SQL** is used.
- All data (bill items & total) is stored **temporarily in browser memory (RAM)** as long as the page is open.
- Once the page is refreshed, memory is cleared, and the bill resets.
- The browser DOM (Document Object Model) acts as a **temporary storage** for displaying old and new data together.

💡 If needed, this can be upgraded to use:
- **localStorage** → Saves data even after page reload.
- **Backend + Database** → For permanent storage across devices.

---

## 🚀 How to Run
1. Download or clone the repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/kirana-bill-calculator.git
