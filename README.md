# X.com UI Clone – Tailwind CSS

A responsive UI layout inspired by X.com (Twitter), built to practice and demonstrate advanced **Tailwind CSS skills**.  
This project focuses on **mobile-first design, responsive layouts, flexbox, and Material Symbols icons**.

---

## 📂 Project Structure


x-com-ui/
├─ index.html
├─ css/
│ └─ output.css
└─ assets/
└─ icons/

---


- `index.html` – Main HTML layout  
- `css/output.css` – Tailwind compiled CSS  
- `assets/icons/` – Custom SVG icons (if any)

---

## 🖥 Layout Overview

### 1️⃣ Mobile (default)

- Single column (`flex-col`)  
- **Left Sidebar & Right Sidebar hidden**  
- Middle feed takes **full width**

### 2️⃣ Desktop (md/lg+)

- Three-column layout (`md:flex-row`)  
  1. **Left Sidebar:** navigation, icons, fractional width (`md:w-1/5`)  
  2. **Middle Feed:** flexible width (`flex-1`)  
  3. **Right Sidebar:** optional info, fractional width (`lg:w-1/5`)  
- Spacing handled via **parent padding (`px-*`)** and **`gap-*`**  
- No fixed `mx-auto` for full-width flex rows (avoids layout distortion)

---

## ⚡ Tailwind CSS Approach

- **Mobile-first design**  
  - Stack items vertically on small screens  
  - Hide sidebars using `hidden md:flex` or `hidden lg:flex`  
- **Flexbox for layout**  
  - `flex flex-col md:flex-row` → responsive row/column switching  
  - `flex-1` → middle feed fills remaining space  
  - `gap-*` → spacing between children  
- **Padding for safe margins**  
  - `px-6` or `px-20` → consistent horizontal spacing  
  - Avoid `mx-auto` on full-width flex containers (does not create visible gaps)  
- **Material Symbols icons**  
  - `text-2xl` + `flex items-center gap-2` for proper alignment

---

## 🎨 Features Implemented

- Left sidebar navigation with icons  
- Middle feed placeholder  
- Right sidebar for extra content  
- Fully responsive: mobile → desktop  
- Padding & gap management for proper spacing  
- Mobile-first, easily extendable for real content  

---

## 🏗 How to Run

1. Clone this repository:

```bash
git clone https://github.com/virat-pod/x-webs.git

```
