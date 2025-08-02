# 🍳 Recipe Preparation Agent

An AI-powered web application built with **Node.js** and **IBM Granite LLM**, designed to turn your available ingredients into smart, complete recipes.

---

## 🚀 Features

- **AI-Powered Recipes**: Enter your ingredients and get full recipes instantly  
- **Step-by-Step Instructions**: Easy-to-follow directions for seamless cooking  
- **Smart Substitutions**: Helpful alternative ingredient suggestions  
- **Cooking Tips**: Pro tips to enhance your dishes  
- **Nutritional Highlights**: Basic nutrition facts for your meal  
- **Modern UI**: Responsive, user-friendly design using Tailwind CSS  
- **Copy Button**: Quickly copy and share recipes  

---

## 🛠️ Tech Stack

- **Backend**: Node.js with Express  
- **AI Integration**: IBM Granite LLM via Watson Machine Learning  
- **Frontend**: HTML, Tailwind CSS, JavaScript  
- **Styling**: Tailwind CSS (with custom styling)

---

## 📦 Getting Started

### Prerequisites

- Node.js (v16 or higher)  
- IBM Cloud account with Watson Machine Learning  
- Watson Machine Learning API credentials

### Installation

1. **Clone the Repository**
   ```bash
   git clone <repository-url>
   cd recipe-preparation-agent
   ```

2. **Install Dependencies**
   ```bash
   npm install
   ```

3. **Configure Environment**
   - Copy `.env.example` to `.env`
   - Fill in your IBM credentials:
     ```
     IBM_WATSON_ML_API_KEY=your_api_key
     IBM_WATSON_ML_URL=https://us-south.ml.cloud.ibm.com
     IBM_WATSON_ML_PROJECT_ID=your_project_id
     ```

4. **Start the App**
   ```bash
   npm start
   ```

5. **Visit in Browser**
   - Navigate to: `http://localhost:5000`

---

## 🔐 Get IBM Watson ML Credentials

1. **Create IBM Cloud Account**
   - Sign up at [IBM Cloud](https://cloud.ibm.com/)

2. **Create Watson Machine Learning Instance**
   - From the IBM Cloud dashboard:  
     - Click **Create Resource** → Search for *Watson Machine Learning*  
     - Select the **Lite** plan (free)

3. **Generate API Key**
   - Go to your service instance → **Service credentials**  
   - Create credentials → Copy the `apikey`

4. **Get Project ID**
   - Visit [Watson Studio](https://dataplatform.cloud.ibm.com/)  
   - Create a new project → Go to project settings → Copy the **Project ID**

---

## ⚙️ How to Use

1. Enter your ingredients (e.g., `tomato, onion, garlic`)  
2. Click **Generate Recipe**  
3. Get:
   - Full recipe with quantities  
   - Cooking steps  
   - Smart substitutions  
   - Tips and nutrition info  
4. Click **Copy** to save or share the recipe

---

## ✨ Example Inputs

| Ingredients                        | Suggested Recipe               |
|-----------------------------------|--------------------------------|
| `tomato, onion, rice`             | Tomato Rice Pilaf              |
| `chicken, garlic, lemon, herbs`   | Herb-Crusted Lemon Chicken     |
| `pasta, mushrooms, cream`         | Creamy Mushroom Pasta          |
| `eggs, spinach, cheese`           | Spinach & Cheese Omelet        |

---

## 📡 API Endpoints

- `GET /` → Main App Page  
- `POST /generate-recipe` → AI recipe generation  
- `GET /health` → Health check

---

## 📁 Project Structure

```
recipe-preparation-agent/
├── server.js              # Express server setup
├── package.json           # App dependencies
├── .env.example           # Env variable template
└── public/
    ├── index.html         # UI template
    ├── js/
    │   └── app.js         # Frontend logic
    └── css/
        └── style.css      # Tailwind + custom CSS
```

---

## 🧠 AI Capabilities in Depth

### Smart Recipe Suggestions
- IBM Granite LLM generates realistic and creative recipes
- Takes ingredient combinations and cuisine logic into account

### Clean Formatting
- Readable and well-structured output
- Key information is clearly highlighted

### Mobile-First Design
- Fully responsive on all devices
- Intuitive layout for any screen size

---

## 🧩 Troubleshooting

### API Key Issues
- Double-check `.env` values  
- Ensure the Watson ML instance is active  
- Confirm Project ID is correct

### Recipe Not Generating?
- Test your internet connection  
- Try using simpler ingredient combinations  
- Check IBM Cloud service status

### Styling or UI Problems
- Confirm Tailwind CSS is loaded  
- Inspect the browser console for errors  
- Refresh and clear browser cache

---

## 🤝 Contributing

1. Fork this repo  
2. Create a new branch for your feature  
3. Commit changes and test thoroughly  
4. Submit a Pull Request (PR)

---

## 📄 License

Licensed under the MIT License. See `LICENSE` file for full details.

---

## 📬 Support

For questions or issues:  
- Refer to the [Troubleshooting](#-troubleshooting) section  
- Check IBM Watson ML [documentation](https://cloud.ibm.com/docs/watson-machine-learning)  
- Or open an issue in the GitHub repo

---

**Built with ❤️ using Node.js, Tailwind CSS, and IBM Granite LLM**
# IBM-CLOUD-EDUNET
>>>>>>> 98a67790a5b569079798b91e89d0b6a4db01d2c8
