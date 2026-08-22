# 🎨 ChromaSense — Smart Colour System Palette Recommendation

> **AI-inspired fashion colour recommendation system that analyzes skin tone from a captured image and suggests personalized colours, outfits, and fashion tips.**

ChromaSense is a modern web-based **personal styling assistant** designed to help users discover colours that complement their natural skin tone.

The application uses **JavaScript, Canvas API, and browser camera capabilities** to capture an image, analyze skin-tone characteristics, classify the complexion, and generate a personalized colour palette with fashion recommendations.

---

## ✨ Live Demo

🚀 **Live Demo:** [Add your deployed project link here]

📂 **GitHub Repository:** [ChromaSense Repository](https://github.com/Naveenpandey2008/Styling-suggestion)

---

## 📸 Project Preview

> Add screenshots/GIFs of your application here to make the repository more visually attractive.

### 🏠 Home Page

![Home Page](screenshots/home.png)

### 📷 Camera & Skin Tone Analysis

![Camera Analysis](screenshots/camera.png)

### 🎨 Personalized Colour Palette

![Colour Recommendations](screenshots/recommendations.png)

---

## 🌟 Features

### 🔐 User Authentication

* User-friendly Login and Signup interfaces
* Account information stored using browser `localStorage`
* Simple client-side authentication flow
* Persistent login experience

### 👤 Gender Selection

Users can select:

* Male
* Female
* Other

This selection can be used to personalize the styling recommendations.

### 📷 Camera Integration

ChromaSense allows users to capture their image directly from their device.

* Uses the browser's `MediaDevices API`
* Requests camera permissions securely
* Supports real-time camera preview
* Captures an image without requiring external applications

### 🧑‍🎨 Skin Tone Analysis

The application processes the captured image using the **Canvas API** to identify skin-tone characteristics.

The detected complexion is categorized into predefined skin-tone groups.

### 🎨 Personalized Colour Recommendations

Based on the detected skin tone, ChromaSense generates a personalized colour palette containing colours that are expected to complement the user's complexion.

### 👕 Fashion Tips

Users also receive styling suggestions and fashion tips related to their detected skin tone.

### 💾 Local Data Storage

User information and application data are stored locally using browser `localStorage`, allowing the project to work without a traditional backend.

---

# 🧠 How ChromaSense Works

The application follows a simple image-processing and recommendation workflow:

```text
        👤 User
           │
           ▼
    🔐 Login / Signup
           │
           ▼
    👤 Select Gender
           │
           ▼
      📷 Open Camera
           │
           ▼
      📸 Capture Photo
           │
           ▼
    🖼️ Canvas Processing
           │
           ▼
    🎨 Skin Tone Detection
           │
           ▼
   🧠 Tone Classification
           │
           ▼
 🎨 Colour Recommendation Engine
           │
           ▼
 👕 Fashion Tips & Suggestions
```

---

# 🎨 Skin Tone Classifications

ChromaSense currently classifies users into six predefined categories:

| Skin Tone          | Description                              |
| ------------------ | ---------------------------------------- |
| 🤎 **Deep**        | Deeper complexion with rich undertones   |
| 🟤 **Medium-Warm** | Medium complexion with warm undertones   |
| 🩷 **Medium-Cool** | Medium complexion with cooler undertones |
| 🟡 **Light-Warm**  | Light complexion with warm undertones    |
| 🔵 **Light-Cool**  | Light complexion with cool undertones    |
| 🤍 **Fair**        | Very light complexion                    |

Each classification is connected to a corresponding set of recommended colours and fashion guidance.

---

# 🛠️ Technology Stack

### Frontend

* **HTML5** — Application structure
* **CSS3** — Styling, layouts, gradients and animations
* **JavaScript** — Application logic and interactivity

### Browser APIs

* **Canvas API** — Image processing and pixel analysis
* **MediaDevices API** — Camera access
* **LocalStorage API** — Client-side data persistence

### Development Tools

* Git
* GitHub
* VS Code
* Modern Web Browser

---

# 💡 Core Technical Concepts

This project demonstrates practical implementation of several frontend and browser technologies:

### JavaScript

Used for:

* DOM manipulation
* Event handling
* Authentication logic
* Image processing
* Recommendation generation
* Dynamic UI updates

### Canvas API

The Canvas API is used to:

1. Capture image data
2. Extract pixel information
3. Process RGB values
4. Analyze skin-tone characteristics
5. Classify the detected complexion

### MediaDevices API

The browser camera is accessed using:

```javascript
navigator.mediaDevices.getUserMedia()
```

This allows the application to access the user's camera after permission is granted.

### LocalStorage

User information and application state can be persisted using:

```javascript
localStorage.setItem()
localStorage.getItem()
```

This allows the application to operate without requiring a database or backend server.

---

# 📁 Project Structure

```text
Styling-suggestion/
│
├── index.html
├── login.html
├── signup.html
│
├── css/
│   └── style.css
│
├── js/
│   ├── script.js
│   ├── auth.js
│   └── recommendation.js
│
├── assets/
│   ├── images/
│   └── icons/
│
├── screenshots/
│   ├── home.png
│   ├── camera.png
│   └── recommendations.png
│
└── README.md
```

> Update the structure above according to your actual repository files.

---

# 🚀 Getting Started

## 1. Clone the Repository

```bash
git clone https://github.com/Naveenpandey2008/Styling-suggestion.git
```

## 2. Navigate to the Project

```bash
cd Styling-suggestion
```

## 3. Run the Application

Since ChromaSense is a frontend project, no complex build process is required.

You can open:

```text
index.html
```

directly in a modern browser.

For the best camera experience, however, it is recommended to run the project through a local development server.

For example, using VS Code's **Live Server** extension.

---

# 📷 Camera Permissions

Camera functionality requires browser permission.

When the user clicks **Open Camera**, the browser requests permission to access the device camera.

For production deployments, camera access generally requires a secure context such as:

```text
HTTPS
```

For local development:

```text
localhost
```

is commonly supported.

---

# 🔒 Privacy

ChromaSense is designed as a client-side application.

* 📷 Camera access requires user permission
* 🖼️ Captured images can be processed locally in the browser
* 💾 Application data is stored using browser `localStorage`
* 🌐 No external backend is required for the current implementation

> **Important:** Always review the current source code before claiming that images or personal information never leave the device.

---

# 🎯 Use Cases

ChromaSense can be useful for:

* 👕 Personal fashion styling
* 🎨 Colour selection
* 🛍️ Shopping assistance
* 👔 Outfit planning
* 💄 Personal styling applications
* 🧑‍🎨 Fashion recommendation platforms
* 💻 Frontend development demonstrations

---

# 📊 Example Recommendation Flow

Suppose the system identifies a user's complexion as:

```text
Skin Tone → Medium-Warm
```

The recommendation engine can generate:

```text
Recommended Colours
────────────────────
• Olive
• Mustard
• Rust
• Warm Beige
• Brown
• Cream
```

Along with styling suggestions such as:

```text
Fashion Tip
Warm earthy colours can complement this complexion
and can be incorporated into casual and formal outfits.
```

---

# 🧪 Browser Compatibility

ChromaSense is designed for modern browsers.

| Browser         | Support       |
| --------------- | ------------- |
| Google Chrome   | ✅ Recommended |
| Microsoft Edge  | ✅ Recommended |
| Mozilla Firefox | ✅ Supported   |
| Safari          | ✅ Supported   |

Camera functionality depends on browser permissions and device capabilities.

---

# ⚡ Key Highlights

* 🎨 Personalized colour recommendations
* 📷 Real-time camera integration
* 🧠 Image-based skin-tone classification
* 🖼️ Canvas-based image processing
* ⚡ Lightweight frontend application
* 🔐 Client-side authentication
* 💾 LocalStorage-based persistence
* 📱 Responsive user interface
* ✨ Modern CSS animations and gradients
* 🚫 No backend or database required

---

# 📈 Future Improvements

The project can be expanded significantly in future versions.

### 🤖 AI-Based Skin Analysis

Replace rule-based classification with a machine-learning or computer-vision model for more robust skin-tone detection.

### 🎨 Undertone Detection

Add dedicated detection for:

* Warm undertone
* Cool undertone
* Neutral undertone

### 👕 Outfit Recommendations

Instead of recommending colours only, the system could recommend complete outfits based on:

* Skin tone
* Gender preference
* Occasion
* Season
* Personal style

### 🛍️ Shopping Integration

Recommended colours could be connected with fashion products from online stores.

### 📱 Mobile Application

The project could be converted into a mobile application using technologies such as:

* React Native
* Flutter

### ☁️ Cloud-Based Accounts

A backend could be added to support:

* Secure authentication
* User profiles
* Saved palettes
* Recommendation history
* Personalized preferences

### 🧠 Advanced Computer Vision

Future versions could use computer-vision models for:

* Face detection
* Better skin-region detection
* Lighting correction
* Undertone analysis
* More accurate colour classification

---

# 🏆 What I Learned

Building ChromaSense helped demonstrate practical knowledge of:

* HTML5 semantic structure
* Advanced CSS styling
* JavaScript DOM manipulation
* Event-driven programming
* Browser APIs
* Camera integration
* Canvas image processing
* RGB colour analysis
* LocalStorage
* Responsive web design
* Client-side application architecture
* Git and GitHub workflow

---

# 🔮 Future Vision

The long-term goal of ChromaSense is to evolve from a simple colour recommendation website into a complete **AI-powered personal styling assistant**.

Future versions could analyze a user's appearance, preferences, occasion, season, and existing wardrobe to generate complete personalized styling recommendations.

```text
             CHROMASENSE
                  │
        ┌─────────┴─────────┐
        ▼                   ▼
   Skin Analysis       User Preferences
        │                   │
        └─────────┬─────────┘
                  ▼
          Recommendation Engine
                  │
       ┌──────────┼──────────┐
       ▼          ▼          ▼
    Colours    Outfits    Fashion Tips
       │          │          │
       └──────────┼──────────┘
                  ▼
        Personalized Style
```

---

# 🤝 Contributing

Contributions and suggestions are welcome.

If you want to improve the project:

1. Fork the repository
2. Create a new branch

```bash
git checkout -b feature/improvement
```

3. Make your changes
4. Commit your changes

```bash
git commit -m "Add new styling recommendation feature"
```

5. Push the branch

```bash
git push origin feature/improvement
```

6. Create a Pull Request

---

# ⭐ Support

If you find this project interesting or useful, consider giving the repository a ⭐ on GitHub.

It helps support the project and encourages further development.

---

# 👨‍💻 Author

**Naveen Pandey**

B.Tech Computer Science & Engineering

Interested in:

* Full-Stack Development
* Software Engineering
* JavaScript
* React
* Web Technologies
* Data & AI-powered Applications

### Connect with me

* 💻 GitHub: [Naveenpandey2008](https://github.com/Naveenpandey2008)
* 💼 LinkedIn: [Add your LinkedIn profile]
* 📧 Email: [Add your email]

---

# 📄 License

This project is available for educational and development purposes.

Add an appropriate open-source license such as **MIT License** if you want others to freely reuse and modify the project.

---

<div align="center">

### 🎨 ChromaSense

**See your colours. Discover your style.**

⭐ If you like this project, consider giving it a star!

</div>
