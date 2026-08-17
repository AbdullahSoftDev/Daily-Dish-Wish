
<div align="center">
  <img
    src="YOUR_HEADER_IMAGE_URL"
    alt="Daily Dish Wish — Smart Cooking & Meal Planning Platform"
    width="100%"
  />
</div>

# 🍽️ Daily Dish Wish — Smart Cooking & Meal Planning Platform

<div align="center">

**Never Wonder What To Cook Again.**

A modern cooking and meal-planning application designed to help users discover dishes, explore quick meals, randomly choose what to cook, and organize meals across an entire week.

<br>

🌐 **[Visit Daily Dish Wish](https://dailydishwish.netlify.app/)**

</div>

---

<div align="center">

[![React](https://img.shields.io/badge/React-19.2.0-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://react.dev/)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6%2B-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Bootstrap](https://img.shields.io/badge/Bootstrap-5.3-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)](https://getbootstrap.com/)
[![jQuery](https://img.shields.io/badge/jQuery-3.6-0769AD?style=for-the-badge&logo=jquery&logoColor=white)](https://jquery.com/)
[![Netlify](https://img.shields.io/badge/Deployed%20on-Netlify-00C7B7?style=for-the-badge&logo=netlify&logoColor=white)](https://www.netlify.com/)
[![Create React App](https://img.shields.io/badge/Create%20React%20App-5.0.1-09D3AC?style=for-the-badge&logo=react&logoColor=white)](https://create-react-app.dev/)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](#-license)

</div>

---

## 🌐 Production Application

**Daily Dish Wish is deployed and accessible as a live production web application.**

<div align="center">

### 🍽️ [Visit Daily Dish Wish](https://dailydishwish.netlify.app/)

**Discover • Plan • Choose • Cook**

</div>

The production deployment provides direct access to the current application without requiring local installation or development setup.

---

## 📌 About

**Daily Dish Wish** is a modern React-based cooking and meal-planning application created to solve a simple but extremely common problem:

> **“What should I cook today?”**

Instead of repeatedly searching for recipes or spending time deciding what to prepare, users can use Daily Dish Wish to quickly discover dishes, browse quick meals, search for specific dishes, randomly select something through **Surprise Me**, and generate a complete weekly meal schedule.

The application combines a clean user interface with interactive meal-selection and planning features to make everyday food decisions faster and more enjoyable.

The project is built around a structured dish dataset containing information such as:

- 🍽️ Dish name
- 🏷️ Food type
- 🧂 Ingredients
- ⏱️ Cooking time
- 📂 Dish category

---

## 🎯 The Problem

Choosing what to cook every day sounds simple, but it can quickly become repetitive.

Users commonly face questions such as:

- What should I cook today?
- What can I prepare quickly?
- What should I make for lunch?
- What should I cook for dinner?
- Which meals should I plan for this week?
- I have no idea what I want to eat.

Traditional recipe websites often require users to already know what they are looking for.

Daily Dish Wish takes a different approach.

Instead of only asking:

> **“What recipe are you searching for?”**

it also allows users to ask:

> **“Just tell me what to cook.”**

---

## 💡 The Solution

Daily Dish Wish provides multiple ways to make a cooking decision.

```text
                         DAILY DISH WISH
                                │
              ┌─────────────────┼─────────────────┐
              │                 │                 │
              ▼                 ▼                 ▼
          🔎 SEARCH         🎲 SURPRISE        📅 PLAN
              │                 │                 │
              ▼                 ▼                 ▼
        Find a Dish       Random Selection   Weekly Schedule
              │                 │                 │
              └─────────────────┼─────────────────┘
                                │
                                ▼
                         🍽️ Choose a Meal
                                │
                                ▼
                           👨‍🍳 Start Cooking
````

---

## ✨ Core Features

### 🎲 Surprise Me

The **Surprise Me** feature is one of the central experiences of Daily Dish Wish.

When users don't know what they want to cook, they can simply let the application choose for them.

The feature randomly selects a dish from the available meal dataset and presents the result through an interactive selection experience.

**Features:**

- 🎲 Random dish selection
- 🔄 Animated selection process
- ⏳ Progressive selection effect
- 🎯 Final dish selection
- 🍽️ Dish information display
- 🎉 Interactive result experience

### Workflow

```
User
 │
 ▼
🎲 Surprise Me
 │
 ▼
Random Dish Pool
 │
 ▼
Animated Selection
 │
 ▼
Final Dish
 │
 ▼
Dish Information
 │
 ▼
🍳 Cook
```

---

### 📅 Weekly Meal Planner

Planning meals for an entire week can remove a lot of daily decision-making.

Daily Dish Wish can generate a structured **7-day meal schedule**.

The weekly planner organizes meals across:

- Monday
- Tuesday
- Wednesday
- Thursday
- Friday
- Saturday
- Sunday

Each day can contain:

- 🍳 Breakfast
- 🍛 Lunch
- 🍽️ Dinner

### Weekly Planning Flow

```
                WEEKLY PLANNER
                      │
        ┌─────────────┼─────────────┐
        ▼             ▼             ▼
    Breakfast       Lunch         Dinner
        │             │             │
        └─────────────┼─────────────┘
                      │
                      ▼
                Daily Schedule
                      │
                      ▼
                 7-Day Plan
```

---

### 🚀 Today's Quick Meals

Sometimes users don't need a complete weekly plan.

They simply need something quick.

The **Today's Quick Meals** section provides a selection of meal suggestions intended to help users quickly decide what to cook.

Each meal can provide information such as:

- 🍽️ Dish name
- 🏷️ Category
- 🥗 Food type
- ⏱️ Cooking time

The selection can change to provide different meal suggestions.

---

### 🔎 Dish Search

Daily Dish Wish includes a search experience for users who already have an idea of what they want.

The search functionality can search through available dishes based on information such as:

- Dish name
- Category
- Food type

### Search Workflow

```
Search Query
     │
     ▼
Normalize Query
     │
     ▼
Search Dataset
     │
     ├──────────────┐
     ▼              ▼
   Name          Category
     │              │
     └──────┬───────┘
            ▼
        Food Type
            │
            ▼
      Matching Results
```

---

### 🥘 Dish Dataset

The application uses a structured local dataset for its meal information.

Each dish contains structured information that can be used throughout the application.

Example:

```
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

This structure allows the same dataset to power multiple application features.

```
                 Dish Dataset
                      │
       ┌──────────────┼──────────────┐
       ▼              ▼              ▼
    Search         Surprise       Planner
       │              │              │
       ▼              ▼              ▼
   Find Dish      Random Dish     Weekly Meal
```

---

### 🥗 Food Type Classification

Meals are categorized according to their food type.

```
                    MEALS
                      │
              ┌───────┴───────┐
              ▼               ▼
             VEG            NON-VEG
              │               │
              ▼               ▼
        Palak Paneer     Chicken Biryani
        Aloo Gobi        Chicken Karahi
        Daal Chawal      Beef Kebab
        Falafel Wrap     Mutton Nihari
```

This classification provides the foundation for food-type filtering and searching.

---

### ⏱️ Cooking Time

Cooking time is stored as part of each dish's information.

This provides users with an additional way to understand how much time a meal may require and provides a foundation for future time-based filtering.

```
Dish
 │
 ├── Name
 ├── Food Type
 ├── Ingredients
 └── Cooking Time
```

---

### 🧂 Ingredient Information

Each dish contains an ingredient list.

This provides the foundation for future features such as:

- 🛒 Smart shopping lists
- 📋 Ingredient-based searching
- 🧮 Ingredient quantity calculation
- 🥘 Recipe preparation
- 🛍️ Grocery planning

---

### 🛒 Interactive Shopping Interface

The application also contains shopping/cart interactions within its interface.

Products can contain information such as:

- Product name
- Price
- Image
- Category

Users can interact with the shopping interface and maintain a cart count.

This provides a foundation for future grocery-oriented functionality.

---

## 🧠 Application Architecture

Daily Dish Wish currently follows a frontend-focused React architecture.

```
┌──────────────────────────────────────────────┐
│              React Application               │
│                                              │
│              Daily Dish Wish                 │
└──────────────────────┬───────────────────────┘
                       │
                       ▼
┌──────────────────────────────────────────────┐
│                    App.js                    │
│                                              │
│ Search │ Surprise │ Planner │ Quick Meals    │
└─────────────┬────────────────┬───────────────┘
              │                │
              ▼                ▼
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
     │ UI & Styling       │
     │                    │
     │ React + Bootstrap  │
     │ CSS + JavaScript   │
     └────────────────────┘
```

---

## 🧩 Application Components

```
src/
│
├── App.js
│   │
│   ├── Navigation
│   ├── Hero Section
│   ├── Search
│   ├── Quick Meals
│   ├── Surprise Me
│   ├── Weekly Planner
│   ├── Dish Information
│   └── Cart Interaction
│
├── dishesData.js
│   │
│   └── Dish Dataset
│       ├── ID
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
├── logo.svg
│   └── Application Logo
│
├── App.test.js
│   └── Application Tests
│
├── setupTests.js
│   └── Testing Configuration
│
└── reportWebVitals.js
    └── Performance Metrics
```

---

## 🏗️ Technology Stack

### Frontend

- ⚛️ **React 19**
- 🟨 **JavaScript ES6+**
- 🌐 **HTML5**
- 🎨 **CSS3**

### UI & Libraries

- 🅱️ **Bootstrap 5.3**
- 💻 **jQuery 3.6**

### Development

- Create React App
- React Scripts
- npm
- Node.js

### Testing

- Jest
- React Testing Library
- DOM Testing Library

### Deployment

- 🌐 **Netlify**

---

## 📦 Project Dependencies

The project uses the React ecosystem with dependencies including:

```
React
React DOM
React Scripts
Bootstrap
jQuery
Testing Library
Jest
Web Vitals
```

Dependency versions are maintained through:

```
package.json
package-lock.json
```

---

## 📁 Project Structure

```
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

Before running the project locally, make sure you have:

- Node.js
- npm
- Git
- A modern web browser

Verify your installation:

```
node --version
npm --version
git --version
```

---

## 1️⃣ Clone the Repository

```
git clone https://github.com/AbdullahSoftDev/Daily-Dish-Wish.git
```

Navigate into the project:

```
cd Daily-Dish-Wish
```

---

## 2️⃣ Install Dependencies

```
npm install
```

---

## 3️⃣ Start Development Server

```
npm start
```

The application will normally be available at:

```
http://localhost:3000
```

---

## 4️⃣ Production Build

Create an optimized production build:

```
npm run build
```

The resulting files will be generated inside:

```
build/
```

---

## 🧪 Testing

Run the test suite:

```
npm test
```

The project includes:

```
App.test.js
setupTests.js
```

Testing tools include:

- Jest
- React Testing Library
- DOM Testing Library

---

## 🌐 Production Deployment

Daily Dish Wish is deployed using **Netlify**.

### Production URL

## 🍽️ [https://dailydishwish.netlify.app/](https://dailydishwish.netlify.app/)

**Live Production Application**

The deployed application provides access to the current production version of Daily Dish Wish.

---

## 🔄 Production Workflow

```
                Source Code
                     │
                     ▼
              GitHub Repository
                     │
                     ▼
              Production Build
                     │
                     ▼
                  Netlify
                     │
                     ▼
          ┌─────────────────────┐
          │ Daily Dish Wish     │
          │ Production Website  │
          └─────────────────────┘
                     │
                     ▼
                 End Users
```

---

## 🎨 User Experience

Daily Dish Wish is built around quick decision-making.

The application avoids forcing users through complicated workflows before they can find something to cook.

The primary experience can be summarized as:

```
              WHAT SHOULD I COOK?
                       │
        ┌──────────────┼──────────────┐
        ▼              ▼              ▼
      SEARCH         SURPRISE        PLAN
        │              │              │
        ▼              ▼              ▼
     Find It       Choose For Me   Plan Week
        │              │              │
        └──────────────┼──────────────┘
                       ▼
                 Select Meal
                       │
                       ▼
                  Start Cooking
```

---

## 📊 Feature Overview

| FeatureStatus                                 |             |
| --------------------------------------------- | ----------- |
| 🔎 Dish Search                                | ✅ Available |
| 🎲 Surprise Me                                | ✅ Available |
| 📅 Weekly Meal Planner                        | ✅ Available |
| 🚀 Quick Meals                                | ✅ Available |
| 🥗 Vegetarian / Non-Vegetarian Classification | ✅ Available |
| ⏱️ Cooking Time                               | ✅ Available |
| 🧂 Ingredient Information                     | ✅ Available |
| 🛒 Cart Interaction                           | ✅ Available |
| ⚛️ React Application                          | ✅ Available |
| 📱 Responsive Interface                       | ✅ Available |
| 🧪 Testing Setup                              | ✅ Available |
| 🌐 Production Deployment                      | ✅ Available |

---

## 🔮 Future Development

Daily Dish Wish has significant potential for expansion.

### 🤖 AI-Powered Recommendations

Future versions can introduce AI-based recommendations that consider:

- User preferences
- Previous meals
- Available ingredients
- Cooking time
- Dietary requirements
- Cuisine preferences
- Meal type
- Seasonal ingredients

```
User Preferences
      │
      ├── Cuisine
      ├── Cooking Time
      ├── Dietary Preference
      └── Meal Type
              │
              ▼
       AI Recommendation
              │
              ▼
       Personalized Meal
```

---

### ❤️ Favorites

Future versions can allow users to save dishes they enjoy.

```
Dish
 │
 ▼
❤️ Add to Favorites
 │
 ▼
Favorites Collection
 │
 ▼
Quick Access
```

---

### 👤 User Accounts

Future versions can introduce accounts for persistent personalization.

Possible functionality:

- User registration
- Login
- Saved dishes
- Favorite meals
- Personalized schedules
- Meal history
- User preferences

---

### 🔍 Advanced Search & Filters

Future search functionality could include:

- Cuisine
- Meal type
- Cooking time
- Difficulty
- Dietary preference
- Ingredients
- Vegetarian
- Non-vegetarian

```
                ADVANCED SEARCH
                       │
        ┌──────────────┼──────────────┐
        ▼              ▼              ▼
     Cuisine         Time          Dietary
        │              │              │
        └──────────────┼──────────────┘
                       ▼
                 Filtered Meals
```

---

### 📝 Custom Dish Creation

Users could eventually create their own dishes by adding:

- Dish name
- Ingredients
- Cooking time
- Category
- Cuisine
- Instructions
- Images

---

### 🎥 Recipe Video Integration

Future versions can connect dishes with cooking videos to provide visual preparation guidance.

```
Dish
 │
 ├── Ingredients
 ├── Cooking Time
 ├── Instructions
 └── 🎥 Video
```

---

### 🛍️ Smart Grocery Lists

The ingredient system can eventually be connected to a smart shopping list.

```
Weekly Meal Plan
       │
       ▼
Recipe Ingredients
       │
       ▼
Combine Ingredients
       │
       ▼
Remove Duplicates
       │
       ▼
🛒 Smart Grocery List
```

---

### 📱 Progressive Web App

Future versions could support PWA functionality, allowing users to:

- Install the application
- Use it from a mobile home screen
- Cache application resources
- Improve offline functionality
- Provide an app-like experience

---

## 🛠️ Development Philosophy

Daily Dish Wish is built around a simple principle:

> **Make deciding what to cook easier.**

The goal isn't to create another complicated recipe website.

The goal is to create a useful cooking companion that helps users move from:

```
🤔 “What should I cook?”
```

to:

```
🍽️ “This looks good.”
```

and finally:

```
👨‍🍳 “Let's cook.”
```

---

## 🔐 Security & Production Considerations

Because the current application is primarily frontend-focused and uses local application data, it does not require a traditional backend authentication system.

For future backend integrations, production deployments should consider:

- Secure API communication
- Environment variables
- Authentication security
- Input validation
- API rate limiting
- Database security
- Secure user sessions
- HTTPS
- Data privacy
- Secure storage of user preferences

---

## 📈 Performance Considerations

The application is designed as a client-side React application.

Potential performance considerations include:

- Efficient component rendering
- Optimized images
- Lazy loading
- Dataset optimization
- Code splitting
- Asset compression
- Browser caching
- Production builds

The production deployment uses an optimized build rather than the development server.

---

## 🤝 Contributing

Contributions, suggestions, improvements, and feature ideas are welcome.

### Development Workflow

Clone the project:

```
git clone https://github.com/AbdullahSoftDev/Daily-Dish-Wish.git
cd Daily-Dish-Wish
```

Create a branch:

```
git checkout -b feature/your-feature
```

Make your changes and test them locally.

Then:

```
git add .
git commit -m "Add your feature"
git push origin feature/your-feature
```

Finally, open a Pull Request.

---

## 🐛 Issues & Suggestions

If you find a bug or have an idea for improving Daily Dish Wish, feel free to open an issue in the GitHub repository.

Useful issue information includes:

- Description of the problem
- Steps to reproduce
- Expected behavior
- Actual behavior
- Browser/device information
- Screenshots when applicable

---

## 📜 License

This project is licensed under the **MIT License**.

See the `LICENSE` file for complete license information.

---

## 👨‍💻 Author

# Muhammad Abdullah

### Full-Stack AI Developer | Computer Science Student

Building practical software across:

**Artificial Intelligence • Full-Stack Development • Web Applications • Software Engineering**

---

## 🌐 Production

# 🍽️ Daily Dish Wish

### **Never Wonder What To Cook Again.**

Discover meals.
Plan your week.
Choose something delicious.

### 🚀 [Visit Daily Dish Wish](https://dailydishwish.netlify.app/)

⭐ **If you like the project, consider giving the repository a star.**

---

### 🍽️ DAILY DISH WISH

**Discover • Plan • Cook • Enjoy**
