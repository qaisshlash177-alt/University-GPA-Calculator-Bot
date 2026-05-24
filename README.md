# 🎓 University GPA Calculator Bot (`@FourZeroGuardBot`)

[![Telegram Bot](https://img.shields.io/badge/Telegram-Bot-blue?style=for-the-badge&logo=telegram)](https://t.me/FourZeroGuardBot)
[![Scale](https://img.shields.io/badge/GPA%20Scale-4.0-🎯%20Gold?style=for-the-badge)](#)

An interactive and feature-rich Telegram Bot tailored for university students to calculate both **Semester and Cumulative GPA** using the standard US/Gulf **4.0 scale**. 

Unlike basic calculators, this bot features advanced, built-in academic logic to intelligently handle **repeated courses**, ensuring that cumulative GPA updates perfectly without duplicating earned credit hours.

---

## 🚀 Live Demo
Try the bot live on Telegram right now:
🔗 **[Click Here to Launch the Bot | @FourZeroGuardBot](https://t.me/FourZeroGuardBot)**

---

## ✨ Core Features

* 📊 **Dual-Mode Calculation:** Computes both Semester and Cumulative GPA based on credit hours and standard letter grades (`A+`, `A`, `B`, etc.).
* 🔄 **Advanced Course-Repeat Logic:**
  * `🆕 New Course:` Credit hours and points are added normally to both semester and cumulative totals.
  * `🔄 Repeat (Raise GPA):` Dynamically subtracts old grade points from the cumulative total and injects the new ones while maintaining stable credit hours.
  * `❌ Repeat (Failed Before):` Overwrites the previous `F` (0.00 pts) seamlessly without double-counting hours.
* 💾 **Persistent User Sessions:** Powered by an embedded database, the bot remembers your past GPA and completed hours. You can add, view, edit, or delete courses dynamically anytime.
* ⌨️ **Interactive UI:** Smooth navigation utilizing interactive Inline Keyboards for data entry.
* 💬 **Student-Friendly Engagement:** Includes engaging, contextual polls at the end of calculations to match the student community vibe (e.g., "منعوض بالفاينل" 😉).

---

## 📸 Bot Interface & User Experience
Here is a live look at how the bot interacts with students seamlessly inside Telegram:

| 1. Main Menu (`/start`) | 2. Data Entry & Grade Selection | 3. Successful Course Insertion |
| :---: | :---: | :---: |
| <img src="https://raw.githubusercontent.com/qaisshlash177-alt/University-GPA-Calculator-Bot/main/68075.jpg" width="230" alt="Main Menu"/> | <img src="https://raw.githubusercontent.com/qaisshlash177-alt/University-GPA-Calculator-Bot/main/68074.jpg" width="230" alt="Grade Selection"/> | <img src="https://raw.githubusercontent.com/qaisshlash177-alt/University-GPA-Calculator-Bot/main/68073.jpg" width="230" alt="Course Added"/> |

---

## 🛠️ Tech Stack & Architecture

Built with production-ready best practices, the bot's backend is lightweight, stable, and highly responsive:

* **Language:** Python 3.x
* **Bot Framework:** `pyTelegramBotAPI` (telebot) utilizing optimized `infinity_polling`.
* **Database & State Management:** `SQLite3` with `Foreign Keys` and `Row Factory` enabled to securely isolate user sessions and prevent multi-user state overlapping.
* **Architecture:** Structured Finite State Machine (FSM) simulation via database fields to handle free-text user inputs smoothly.

---

## 🎯 Grading Scale Mapping Table

The bot utilizes the following standard point distribution:

| Grade | Points | | Grade | Points |
| :---: | :---: | :---: | :---: | :---: |
| **A+** | 4.00 | | **C+** | 2.50 |
| **A** | 3.75 | | **C** | 2.25 |
| **A-** | 3.50 | | **C-** | 2.00 |
| **B+** | 3.25 | | **D+** | 1.75 |
| **B** | 3.00 | | **D** | 1.50 |
| **B-** | 2.75 | | **F** | 0.00 |

---

## 📞 Contact & Support
If you have any questions, suggestions, or feature requests, feel free to reach out:
* **Developer:** QAIS SHLASH
* **Telegram:** [🔗 @qaisshlash](https://t.me/qaisshlash)
* 
