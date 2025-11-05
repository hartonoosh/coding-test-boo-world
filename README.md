# Boo Technical Test – Commenting & Voting Feature

This project is a submission for the **Boo Web Developer Technical Test**.  
The goal of the task is to **enhance the given static page** by adding interactive features such as **commenting**, **voting**, **filtering**, and **sorting**, based on the provided **Figma design** and instructions.

---

## Features Implemented

### Voting
- Users can vote on the celebrity's **personality type** across 3 systems:
  - **MBTI:** INFP, INFJ, ENFP, ENFJ, INTJ, INTP, ENTP, ENTJ, ISFP, ISFJ, ESFP, ESFJ, ISTP, ISTJ, ESTP, ESTJ  
  - **Enneagram:** 1w2, 2w3, 3w2, 3w4, 4w3, 4w5, 5w4, 5w6, 6w5, 6w7, 7w6, 7w8, 8w7, 8w9, 9w8, 9w1  
  - **Zodiac:** Aries, Taurus, Gemini, Cancer, Leo, Virgo, Libra, Scorpio, Sagittarius, Capricorn, Aquarius, Pisces
- Each tag starts at **30% opacity**.
- When selected, a dropdown appears to choose a personality type.
- After selection, the tag changes to **100% opacity** to indicate an active vote.

---

### Commenting
- A **Vote/Comment** button triggers the comment input box.
- Users can type a comment and optionally select a personality type.
- The **Submit button** turns **blue (#4EDCD8)** when:
  1. A personality type is selected (MBTI / Enneagram / Zodiac), or  
  2. The user starts typing a title or description.
- Upon submitting:
  - Borders **glow blue (#4EDCD8)** for 1 second.
  - The new comment appears **in real-time** without page reload.

---

### Like Button
- Clicking the like button turns it **blue (#4EDCD8)**.
- Clicking again “unlikes” it and reverts to **gray (#6B6A6A)**.
- Like counts update instantly with a smooth animation.

---

### Filter & Sorting
- **Filter:** Filter comments based on selected personality system (MBTI, Enneagram, Zodiac).  
- **Sorting:**
  - **Recent:** Sorts comments by newest first.
  - **Best:** Sorts comments by number of likes.
- The screen **updates dynamically with animations** when the user applies filters or sorts.

---

### Real-Time UI Updates
- All interactions (commenting, voting, liking, sorting, filtering) are handled **client-side**.
- Data is stored **in memory** (no backend persistence).
- Smooth **transition animations** are added to enhance UX.

---

## Tech Stack
- **Frontend:** HTML, CSS, JavaScript 
- **Backend (Static Mock Server):** Node.js + Express  
- **UI Animations:** CSS transitions  
- **Data Storage:** Client-side (in-memory)

---

## Setup Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/hartonoosh/coding-test-boo-world.git
   cd coding-test-boo-world
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the server:
   ```bash
   npm start
   ```
   The app will run at:  
   [http://localhost:3000](http://localhost:3000)

---

## Notes
- No authentication or user system was implemented as per the test requirements.  
- Name and profile picture of commenters are **hard-coded**.  
- All interactions are **instant and animated** without needing to refresh the page.

---

## Figma Reference
All UI and behavioral details were implemented based on the provided Figma design and accompanying instructions.

---

## Author
**Sri Hartono**  
Web Developer  
📧 [srihartono@gmail.com]  
🔗 [https://hartonoosh.github.io/]
