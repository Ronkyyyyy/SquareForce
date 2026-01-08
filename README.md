# SQUARE FORCE (スクエア・フォース)

![Version](https://img.shields.io/badge/version-1.3.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![React](https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat&logo=vite&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat&logo=tailwind-css&logoColor=white)

**[English](#english) | [日本語](#japanese)**

---

<a name="english"></a>
## 🇬🇧 English

### 🌌 Overview
**SQUARE FORCE** is a strategic board game where physics meets psychology.
Four forces (North, South, East, West) compete to push a central "Core" into opponents' territories using vector mechanics.

This web application features the complete base game along with advanced expansion modules like **"Gravity Shift"** and **"Secret Alliance"**.

👉 **[Play Demo Here](https://your-demo-url.vercel.app)** (Replace with your link)

### 🎮 Game Features

#### 1. Core Mechanics
* **Vector Battle:** Movement is determined by the difference between opposing forces. (e.g., North `5` vs South `2` = Move `3` North).
* **Zero Impact (Warp):** If forces cancel out perfectly (Net 0), the Core **warps** to the point-symmetric position.
    * *Gravity Shock:* If Net 0 happens at the center, all players take 1 damage.
* **River Draft System:** Played cards flow to the left neighbor, creating a unique resource circulation. "Poisoning" your neighbor's hand is a key strategy.

#### 2. Expansion: Gravity Shift (Physics Change)
The physics of the Core change in a fixed cycle every time it falls out of bounds.

1.  **Standard:** Normal rules.
2.  **Rapid:** Movement +1 (if moving). Speed increases, preventing stagnation.
3.  **Heal:** **Recovery Mode.**
    * Side Fall: The owner **gains +1 HP**.
    * Corner Fall: **0 Damage** (Neutral).
    * *Pulling the Core into your own territory is the strategy here.*
4.  **Bomb:** **Double Damage.** (Side: 4 Dmg, Corner: 2 Dmg).

#### 3. Expansion: Secret Alliance (Hidden Roles)
A 2v2 team battle mode where partners are unknown.

* **Win Condition:** Eliminate the opposing team.
* **Insight:** When taking damage, you can secretly view **one player's role**.
* **Blind Parade (Option):**
    * Players start with **ZERO information** (don't even know their own role).
    * Taking damage allows you to check **Any player's role (including Self)**.
    * *Will you seek your identity, or spy on others?*

### 🛠 Tech Stack
* **Framework:** React
* **Build Tool:** Vite
* **Styling:** Tailwind CSS
* **Icons:** Lucide React

### 🚀 Local Setup

```bash
# Clone the repository
git clone [https://github.com/your-username/square-force.git](https://github.com/your-username/square-force.git)

# Navigate to directory
cd square-force

# Install dependencies
npm install

# Run development server
npm run dev
