# 🧑‍💻 Frontend Wizards — Stage 0 Task: Profile Card

Welcome to my Stage 0 submission for **HNG Frontend Wizards**! 🚀  
This project implements a fully accessible, responsive **Profile Card** built with **HTML, CSS, and Vanilla JavaScript** following the official task requirements.

---

## 📋 Task Overview

The goal was to create a semantic, testable, and visually appealing **Profile Card** that displays user information such as name, avatar, bio, current time, social links, hobbies, and dislikes.

All elements include the required `data-testid` attributes for automated testing.

### ✅ Core Requirements Implemented

| Feature | Description | Status |
|----------|--------------|--------|
| **Profile Card Container** | Root container for the card (`data-testid="test-profile-card"`) | ✅ |
| **User Name** | Displays the user’s name (`data-testid="test-user-name"`) | ✅ |
| **Biography** | A short bio paragraph (`data-testid="test-user-bio"`) | ✅ |
| **Current Time** | Displays live time in milliseconds (`data-testid="test-user-time"`) | ✅ |
| **Avatar** | User profile image (`data-testid="test-user-avatar"`) | ✅ |
| **Social Links List** | Navigation list of social links (`data-testid="test-user-social-links"`) | ✅ |
| **Individual Social Links** | Twitter, GitHub, LinkedIn with their own `data-testid`s | ✅ |
| **Hobbies List** | Displays hobbies (`data-testid="test-user-hobbies"`) | ✅ |
| **Dislikes List** | Displays dislikes (`data-testid="test-user-dislikes"`) | ✅ |
| **Responsive Design** | Works seamlessly on mobile, tablet, and desktop | ✅ |
| **Keyboard Accessibility** | All links focusable and usable via keyboard | ✅ |

---

## 🧱 Tech Stack

- **HTML5** (Semantic structure)
- **CSS3** (Flexbox + Grid for responsiveness)
- **Vanilla JavaScript (ES6)** (Dynamic time updates)
- **Accessible Design** (Alt text, focus styles, ARIA labels)

---

> The layout adapts fluidly to all screen sizes — mobile, tablet, and desktop.

---

## 🕒 Dynamic Time Feature

The profile card displays the **current time in milliseconds**, updating every second:
```js
const timeEl = document.querySelector('[data-testid="test-user-time"]');
timeEl.textContent = Date.now();
