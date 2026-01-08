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

```

---

<a name="japanese"></a>

## 🇯🇵 日本語

### 🌌 概要

**SQUARE FORCE（スクエア・フォース）** は、物理法則と心理戦が融合した戦略ボードゲームです。
東西南北の4つの勢力が、中央にある「コア」を互いの陣地に押し合う、ベクトル演算バトルです。

本アプリは、基本ルールに加え、物理法則が変化する「グラビティ・シフト」や、正体隠匿モード「シークレット・アライアンス」を完全実装しています。

👉 **[デモをプレイする](https://www.google.com/url?sa=E&source=gmail&q=https://your-demo-url.vercel.app)** （ここにURLを入れてください）

### 🎮 ゲームの特徴

#### 1. 基本システム

* **ベクトル・バトル:** 向かい合うプレイヤーの数値の「差分」でコアが移動します。（例：北`5` vs 南`2` ＝ 北へ`3`マス移動）
* **ゼロ・インパクト (Warp):** 力が完全に拮抗（移動量0）すると、コアが点対称の位置へ**ワープ**します。
* *グラビティ・ショック:* 中心で拮抗した場合は、全員が1ダメージを受けます。


* **リバー・ドラフト:** 使用したカードは左隣のプレイヤーへ流れます。「誰に何を流すか」が重要な戦略となります。

#### 2. 拡張：グラビティ・シフト (物理変動)

コアが盤外へ落ちるたびに、物理法則が以下のサイクルで変化します。

1. **Standard (標準):** 通常ルール。
2. **Rapid (加速):** 移動力+1（動く場合のみ）。実力勝負が加速します。
3. **Heal (癒やし):** **回復モード。**
* 辺落ち：担当者は **HP+1回復**。
* 角落ち：**ダメージ無効 (±0)**。
* *このフェーズのみ、コアを自分の陣地に引き込むことが利益になります。*


4. **Bomb (爆発):** **ダメージ2倍。** 決着をつけるクライマックスです。

#### 3. 拡張：シークレット・アライアンス (正体隠匿)

誰が味方か分からない状態で戦う、2対2のチーム戦モードです。

* **勝利条件:** 敵チームの誰かを脱落させること。
* **インサイト:** ダメージを受けた際、**誰か1人の正体**をこっそり見ることができます。
* **Blind Parade (上級オプション):**
* **「自分の正体すら分からない」**状態でスタートします。
* ダメージを受けた際、**「自分を含む全員」**の中から1人を選んで正体を確認できます。
* *まずは自分を知るか、他人を探るか。戦術が試されます。*



### 🛠 使用技術

* **Framework:** React
* **Build Tool:** Vite
* **Styling:** Tailwind CSS
* **Icons:** Lucide React

### 🚀 インストール方法

```bash
# リポジトリをクローン
git clone [https://github.com/your-username/square-force.git](https://github.com/your-username/square-force.git)

# ディレクトリへ移動
cd square-force

# 依存関係のインストール
npm install

# ローカルサーバーの起動
npm run dev

```

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](https://www.google.com/search?q=LICENSE) file for details.

## 👤 Author

* **[Your Name]** - *Initial work*

```

```
