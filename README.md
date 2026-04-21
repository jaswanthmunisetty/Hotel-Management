# 🏨 Hotel Management System

A terminal-based Hotel Management System built in **Java** that handles room booking, food ordering, billing and data persistence — demonstrating core Java concepts like OOP, Multithreading, Serialization and File I/O.

---

## 🎯 What Does It Do?

A complete hotel management system that runs in the terminal where staff can:
- Book rooms for customers
- Order food to rooms
- Generate bills at checkout
- Save and restore all data automatically

---

## ✨ Features

| Feature | Description |
|---|---|
| 🏠 **Room Booking** | Book any available room with customer details |
| 🍕 **Food Ordering** | Order food items directly to the room |
| 💰 **Auto Billing** | Automatically calculates room + food charges |
| 🚪 **Checkout** | Deallocates room and generates final bill |
| 📋 **Room Availability** | Check available rooms in real time |
| 💾 **Data Backup** | Saves all data to file automatically |
| 🔄 **Data Restore** | Loads saved data when program restarts |
| ⚡ **Background Saving** | Uses Java Thread to save data without blocking |

---

## 🏠 Room Types & Pricing

| Room Type | Rooms Available | Price Per Day |
|---|---|---|
| Luxury Double Room | 10 (Room 1-10) | ₹4000 |
| Deluxe Double Room | 20 (Room 11-30) | ₹3000 |
| Luxury Single Room | 10 (Room 31-40) | ₹2200 |
| Deluxe Single Room | 20 (Room 41-60) | ₹1200 |

---

## 🍕 Food Menu

| Item | Price |
|---|---|
| Sandwich | ₹50 |
| Pasta | ₹60 |
| Noodles | ₹70 |
| Coke | ₹30 |

---

## 🛠️ Java Concepts Used

| Concept | How It Is Used |
|---|---|
| **Inheritance** | `Doubleroom extends Singleroom` |
| **Serialization** | Saving and loading hotel data to file |
| **Multithreading** | Background file saving using `Thread` |
| **Custom Exception** | `NotAvailable` exception for booked rooms |
| **ArrayList** | Storing food orders per room |
| **File I/O** | Reading and writing backup file |
| **OOP** | Classes for Food, Singleroom, Doubleroom, Hotel |
| **Switch Case** | Menu driven program navigation |

---

## 📁 Project Structure

```
HotelManagementSystem/
  └── Main.java        # Complete source code
      ├── Food         # Food item class
      ├── Singleroom   # Single room class
      ├── Doubleroom   # Double room (extends Singleroom)
      ├── NotAvailable # Custom exception class
      ├── holder       # Holds all room arrays
      ├── Hotel        # Core hotel operations
      ├── write        # Runnable class for file saving
      └── Main         # Entry point
```

---

## ▶️ How to Run

### Prerequisites
- Java JDK installed ([java.com](https://java.com))
- Any terminal or IDE (VS Code, IntelliJ, Eclipse)

### Step 1: Clone the repository
```bash
git clone https://github.com/your-username/hotel-management-system.git
cd hotel-management-system
```

### Step 2: Compile the code
```bash
javac Main.java
```

### Step 3: Run the program
```bash
java Main
```

---

## 🖥️ Menu Options

```
1. Display room details      → View features and price of room type
2. Display room availability → Check how many rooms are available
3. Book room                 → Book a room with customer details
4. Order food                → Order food items to a room
5. Checkout                  → Generate bill and free up the room
6. Exit                      → Save data and exit
```

---

## 📋 Sample Usage

```
Enter your choice:
3                          ← Book a room

Choose room type:
1. Luxury Double Room
2. Deluxe Double Room
3. Luxury Single Room
4. Deluxe Single Room
1                          ← Luxury Double Room

Choose room number from: 1, 2, 3, 4...
Enter room number: 1

Enter customer name: Jaswanth
Enter contact number: 9999999999
Enter gender: Male
Enter second customer name: Rahul
Enter contact number: 8888888888
Enter gender: Male

Room Booked ✅
```

---

## 💰 Sample Bill

```
*******
 Bill:-
*******

Room Charge - 4000

===============
Food Charges:-
===============
Item       Quantity    Price
-------------------------
Sandwich   2           100.0
Pasta      1           60.0
Coke       3           90.0

Total Amount - 4250.0
```

---

## 💾 Data Persistence

- All hotel data is saved to a file called `backup` automatically on exit
- When the program restarts, it loads all previous bookings from `backup`
- Saving happens in a **background thread** so the program does not freeze
- Uses Java **Serialization** (`ObjectOutputStream` / `ObjectInputStream`)

---

## 🔮 Future Improvements

- [ ] GUI using Java Swing
- [ ] MySQL database instead of file storage
- [ ] Search customer by name or contact
- [ ] Room availability chart
- [ ] Multi-day booking with date tracking
- [ ] Admin login system

---

## 🎓 Concepts Demonstrated

This project is ideal for showcasing the following Java concepts in interviews:

**OOP:**
- Inheritance (`Doubleroom extends Singleroom`)
- Encapsulation (class fields and methods)
- Polymorphism (method overriding)

**Advanced Java:**
- Serialization for data persistence
- Multithreading with `Runnable` interface
- Custom Exception handling
- ArrayList for dynamic food orders
- File I/O with streams

---

## 📄 License

MIT License — free to use and modify!

---

## 👨‍💻 Author

**Jaswanth Munisetty**
- GitHub: [@jaswanthmunisetty](https://github.com/jaswanthmunisetty)

---

> ⭐ If you found this project useful, please give it a star on GitHub!
