<div align="center">
  <img
    src="YOUR_HEADER_IMAGE_URL"
    alt="Daily Dish Wish — Smart Cooking & Meal Planning Platform"
    width="100%"
  />
</div>

# 🍽️ Daily Dish Wish — Smart Cooking & Meal Planning Platform

<div align="center">

**Your intelligent cooking companion for discovering meals, planning your week, and finally answering the question — “What should I cook today?”**

[![React](https://img.shields.io/badge/React-19.2.0-61DAFB?style=for-the-badge\&logo=react\&logoColor=black)](https://react.dev/)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6%2B-F7DF1E?style=for-the-badge\&logo=javascript\&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Bootstrap](https://img.shields.io/badge/Bootstrap-5.3-7952B3?style=for-the-badge\&logo=bootstrap\&logoColor=white)](https://getbootstrap.com/)
[![jQuery](https://img.shields.io/badge/jQuery-3.6-0769AD?style=for-the-badge\&logo=jquery\&logoColor=white)](https://jquery.com/)
[![Create React App](https://img.shields.io/badge/Create%20React%20App-5.0.1-09D3AC?style=for-the-badge\&logo=react\&logoColor=white)](https://create-react-app.dev/)

</div>

---

## 📌 About

**Daily Dish Wish** is a React-based cooking and meal-discovery application designed to make everyday meal decisions easier.

Instead of spending time wondering what to cook, users can explore quick meals, search dishes, randomly discover something through **Surprise Me**, or generate a complete **weekly meal schedule**.

The application combines a recipe-focused interface with lightweight interactive planning features to create a simple and engaging cooking experience.

The project currently uses a structured local dish database containing information such as dish name, dietary type, ingredients, and cooking time.

---

## ✨ Key Features

### 🎲 Surprise Me

Can't decide what to cook?

The **Surprise Me** feature randomly selects a dish from the available quick-meal database.

The experience includes:

* 🎯 Random dish selection
* 🔄 Animated selection process
* ⏳ Progressive slowing effect
* 🎉 Celebration animation when a dish is selected
* 🍽️ Selected dish information

The feature is implemented directly in the React application using component state and timed selection logic.

```text
User
  │
  ▼
🎲 Surprise Me
  │
  ▼
Random Dish Selection
  │
  ▼
Animated Selection
  │
  ▼
🎯 Final Dish
  │
  ▼
Dish Information
```

---

### 📅 Weekly Meal Schedule

Planning meals for an entire week can be difficult.

Daily Dish Wish can generate a **seven-day meal schedule** containing:

* Monday
* Tuesday
* Wednesday
* Thursday
* Friday
* Saturday
* Sunday

Each day can receive:

* 🍳 Breakfast
* 🍛 Lunch
* 🍽️ Dinner

The current implementation generates the schedule by shuffling available quick meals and assigning them across the week.

```text
              Weekly Planner
                    │
       ┌────────────┼────────────┐
       ▼            ▼            ▼
   Breakfast      Lunch        Dinner
       │            │            │
       └────────────┼────────────┘
                    │
                    ▼
              7-Day Schedule
```

---

### 🚀 Today's Quick Meals

The application provides a dedicated **Today's Quick Meals** section.

A selection of meals is randomly generated when the application loads, giving users a fresh set of meal suggestions without manually searching through the entire collection.

Each meal includes information such as:

* Dish name
* Category
* Vegetarian / Non-Vegetarian type
* Estimated preparation time

---

### 🔎 Dish Search

Users can search for dishes directly from the interface.

The search system checks:

* 🍽️ Dish name
* 🏷️ Category
* 🥗 Food type

The interface displays the top matching results and allows the user to select a dish for further viewing.

```text
Search Query
     │
     ▼
Normalize Query
     │
     ▼
Search Dish Database
     │
     ├── Name
     ├── Category
     └── Food Type
     │
     ▼
Top Matching Results
```

---

### 🥘 Dish Information

The project includes structured dish data with information including:

* Unique dish ID
* Dish name
* Food type
* Ingredients
* Cooking time

The current dataset contains examples such as **Chicken Biryani, Chicken Karahi, Palak Paneer, Beef Seekh Kebab, Chicken Shawarma, Vegetable Pulao, Mutton Nihari, Chana Masala, Grilled Fish, Aloo Gobi, Chicken Tikka, Falafel Wrap, Beef Burger, Daal Chawal, and Mutton Korma**.

Example data structure:

```javascript
{
  id: 1,
  name: "Chicken Biryani",
  type: "non-veg",
  ingredients: [
    "basmati rice",
    "chicken",
    "yogurt",
    "onions",
    "biryani spices",
    "saffron",
    "mint",
    "lemon"
  ],
  cookingTime: 60
}
```

---

### 🥗 Vegetarian & Non-Vegetarian Meals

Meals contain a food-type classification that allows the application to distinguish between:

```text
                 Meals
                   │
          ┌────────┴────────┐
          ▼                 ▼
        VEG              NON-VEG
          │                 │
   Palak Paneer        Chicken Biryani
   Aloo Gobi           Chicken Karahi
   Daal Chawal         Beef Kebab
   Falafel Wrap        Mutton Nihari
```

This classification is also used by the search functionality.

---

### 🛒 Interactive Shopping UI

The application also contains product/cart interaction within its interface.

Products are represented with:

* Product name
* Price
* Image
* Category

The React application maintains a cart count and provides an **Add to Cart** interaction.

---

## 🧠 Smart Cooking Workflow

Daily Dish Wish brings the core features together into a simple workflow:

```text
                    DAILY DISH WISH
                           │
          ┌────────────────┼────────────────┐
          │                │                │
          ▼                ▼                ▼
      🔎 Search        🎲 Surprise       📅 Plan
          │                │                │
          ▼                ▼                ▼
       Find Dish        Random Dish     Weekly Meals
          │                │                │
          └────────────────┼────────────────┘
                           │
                           ▼
                    🍽️ Cook Something
```

---

## 🏗️ Architecture

Daily Dish Wish is built as a **React single-page application** using component state and local JavaScript data.

```text
┌──────────────────────────────────────────────┐
│              React Application               │
│                                              │
│          Daily Dish Wish Interface           │
└──────────────────────┬───────────────────────┘
                       │
                       ▼
┌──────────────────────────────────────────────┐
│                 App.js                       │
│                                              │
│ Search │ Surprise │ Planner │ Quick Meals    │
└─────────────┬──────────────┬─────────────────┘
              │              │
              ▼              ▼
     ┌────────────────┐ ┌────────────────────┐
     │ React State    │ │ dishesData.js      │
     │                │ │                    │
     │ Search Results │ │ Dish Information   │
     │ Selected Dish  │ │ Ingredients        │
     │ Weekly Plan    │ │ Cooking Time       │
     │ Quick Meals    │ │ Food Type          │
     └────────────────┘ └────────────────────┘
              │
              ▼
     ┌────────────────────┐
     │ Bootstrap / CSS    │
     │                    │
     │ Responsive UI      │
     └────────────────────┘
```

---

## 🧩 Core Components

```text
src/
│
├── App.js
│   │
│   ├── Quick Meals
│   ├── Weekly Schedule
│   ├── Surprise Me
│   ├── Dish Search
│   ├── Selected Dish
│   └── Cart Interaction
│
├── dishesData.js
│   │
│   └── Dish Dataset
│       ├── Name
│       ├── Type
│       ├── Ingredients
│       └── Cooking Time
│
├── App.css
│   └── Application Styling
│
├── index.css
│   └── Global Styling
│
├── index.js
│   └── React Entry Point
│
└── logo.svg
    └── Application Logo
```

The current repository contains these source files alongside the standard Create React App files.

---

## 🧰 Technology Stack

### Frontend

* **React 19.2.0**
* **JavaScript**
* **HTML5**
* **CSS3**

### UI & Styling

* **Bootstrap 5.3**
* **jQuery 3.6**

### Development

* **Create React App**
* **React Scripts 5.0.1**
* **React Testing Library**
* **Jest**

The dependency configuration currently lists React 19.2.0, React DOM 19.2.0, Bootstrap 5.3.0, jQuery 3.6.0, testing libraries, and React Scripts 5.0.1.

---

## 📁 Project Structure

```text
Daily-Dish-Wish/
│
├── public/
│   └── Public assets
│
├── src/
│   ├── App.js
│   ├── App.css
│   ├── App.test.js
│   ├── dishesData.js
│   ├── index.css
│   ├── index.js
│   ├── logo.svg
│   ├── reportWebVitals.js
│   └── setupTests.js
│
├── .gitattributes
├── .gitignore
├── package.json
├── package-lock.json
├── prompts.txt
└── README.md
```

---

## 🚀 Getting Started

### Requirements

Make sure you have installed:

* **Node.js**
* **npm**
* A modern web browser

---

### 1. Clone the Repository

```bash
git clone https://github.com/AbdullahSoftDev/Daily-Dish-Wish.git
```

Navigate to the project:

```bash
cd Daily-Dish-Wish
```

---

### 2. Install Dependencies

```bash
npm install
```

The project dependencies are defined in `package.json`.

---

### 3. Start Development Server

```bash
npm start
```

The application runs in development mode and is available at:

```text
http://localhost:3000
```

Create React App's development workflow automatically reloads the application when source files are modified.

---

## 🏭 Production Build

Create an optimized production build using:

```bash
npm run build
```

The production files are generated inside:

```text
build/
```

The Create React App build process bundles and optimizes the application for deployment.

---

## 🧪 Testing

Run the project's test suite:

```bash
npm test
```

The repository includes:

```text
App.test.js
setupTests.js
```

and uses React Testing Library and Jest through the project's configured dependencies.

---

## 🎨 User Experience

The application is designed around a simple idea:

> **Don't spend your time wondering what to cook.**

Instead, users can immediately:

```text
🔎 Search a dish
      ↓
🎲 Let the app choose
      ↓
📅 Plan the week
      ↓
🚀 Pick a quick meal
      ↓
🍳 Start cooking
```

The main hero section communicates this directly with the message:

**“Never Wonder What To Cook Again.”**

---

## 📊 Current Feature Overview

| Feature                         | Status |
| ------------------------------- | ------ |
| 🔎 Dish Search                  | ✅      |
| 🎲 Surprise Me                  | ✅      |
| 📅 Weekly Schedule              | ✅      |
| 🚀 Daily Quick Meals            | ✅      |
| 🥗 Veg / Non-Veg Classification | ✅      |
| ⏱️ Cooking Time                 | ✅      |
| 🧂 Ingredient Information       | ✅      |
| 🛒 Cart Interaction             | ✅      |
| ⚛️ React UI                     | ✅      |
| 📱 Responsive UI                | ✅      |
| 🧪 React Testing Setup          | ✅      |

---

## 🔮 Future Improvements

Potential improvements for future versions include:

* ❤️ Favorite dishes
* 👤 User accounts
* 🔐 Authentication
* ☁️ Cloud-based recipe storage
* 📝 Custom dish creation
* 🔍 Advanced filters
* 🌎 Cuisine-based filtering
* ⏱️ Cooking-time filtering
* 🥗 Dietary preference filters
* 📖 Full recipe instructions
* 🎥 Recipe video integration
* 🛒 Smart ingredient shopping lists
* 📅 Persistent weekly meal plans
* 💾 LocalStorage / cloud persistence
* 🤖 AI-powered meal recommendations
* 📊 Personalized cooking suggestions
* 📱 Progressive Web App support

---

## 🛠️ Development Philosophy

Daily Dish Wish focuses on combining **simple interactions with practical automation**.

Rather than overwhelming users with complicated recipe-management workflows, the application provides fast paths to useful decisions:

```text
             ┌───────────────────┐
             │   What to Cook?   │
             └─────────┬─────────┘
                       │
          ┌────────────┼────────────┐
          ▼            ▼            ▼
       Search       Surprise      Schedule
          │            │            │
          └────────────┼────────────┘
                       ▼
                 Choose a Meal
                       │
                       ▼
                    Cook 🍳
```

---

## ⚠️ Project Status

This repository is an actively developed **React-based cooking and meal-planning project**.

The current implementation is primarily frontend-focused, with dish information and quick-meal data maintained within the application source.

---

## 🤝 Contributing

Contributions, ideas, improvements, and feature suggestions are welcome.

### Development Workflow

```bash
git clone https://github.com/AbdullahSoftDev/Daily-Dish-Wish.git

cd Daily-Dish-Wish

git checkout -b feature/your-feature
```

After making your changes:

```bash
git add .

git commit -m "Add your feature"

git push origin feature/your-feature
```

Then open a Pull Request.

---

## 👨‍💻 Author

<div align="center">

### Muhammad Abdullah

**Full-Stack AI Developer | Computer Science Student**

Building practical software across:

**AI • Full-Stack Development • Web Applications • Software Engineering**

[GitHub](https://github.com/AbdullahSoftDev)

</div>

---

<div align="center">

### 🍽️ DAILY DISH WISH

**Discover. Plan. Cook. Enjoy.**

⭐ If you like the project, consider giving the repository a star.

</div>
