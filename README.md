
# 🧠 Smart Resume Builder

A full-stack web application that enables users to create, edit, preview, and download professional resumes with the help of AI, customizable templates, and real-time validation.

## 📑 Table of Contents
- [📌 Features](#-features)
- [🛠️ Tech Stack](#️-tech-stack)
- [📁 Project Structure](#-project-structure)
- [🚀 Installation](#-installation)
- [⚙️ Core Functionalities](#-core-functionalities)
- [🔐 Error Handling & Data Validation](#-error-handling--data-validation)
- [🧩 Component Integration](#-component-integration)
- [🧪 Code Quality & Innovation](#-code-quality--innovation)
- [📄 Future Enhancements](#-future-enhancements)
- [🧑‍💻 Contributors](#-contributors)
- [📜 License](#-license)

## 📌 Features
- ✅ Intuitive resume builder with form input
- 🖼️ Real-time resume preview
- 🎨 Multiple customizable resume templates
- 💡 AI-generated summaries and job descriptions
- 📄 Export resume as PDF
- ✅ Input validation (frontend & backend)
- 🔄 Resume version history (optional)
- 🧠 ATS keyword optimization (planned)

## 🛠️ Tech Stack

| Layer       | Technology                    |
|-------------|-------------------------------|
| Frontend    | React, Tailwind CSS, Formik   |
| Backend     | Node.js, Express.js           |
| Database    | MongoDB (Mongoose ORM)        |
| AI Support  | OpenAI API (optional)         |
| PDF Export  | html2pdf.js                   |
| Validation  | Yup (client), Joi (server)    |

## 📁 Project Structure
```
smart-resume-builder/
├── client/                  # React frontend
│   └── src/
│       ├── components/      # Reusable components
│       ├── pages/           # Pages
│       ├── styles/          # Tailwind/custom styles
│       └── utils/           # Validation, helpers
├── server/                  # Express backend
│   ├── controllers/         # Business logic
│   ├── models/              # Mongoose schemas
│   ├── routes/              # API routes
│   └── app.js               # Server entry
```

## 🚀 Installation
```bash
# 1. Clone repository
git clone https://github.com/your-username/smart-resume-builder

# 2. Setup server
cd smart-resume-builder/server
npm install
touch .env
# Add MONGO_URI and OPENAI_API_KEY in .env
npm start

# 3. Setup client
cd ../client
npm install
npm start
```

## ⚙️ Core Functionalities

### 1. Resume Builder Form
- Capture user details like name, education, skills, and experience.
- Uses Formik + Yup for form management and validation.

### 2. Live Preview
- Real-time rendering of resume data as you type.

### 3. Resume Templates
- Switchable layout/themes using CSS classes or Tailwind utility styles.

### 4. AI Integration
- Generate summaries, job descriptions, or achievements using GPT.

### 5. Export as PDF
- One-click download with html2pdf.js.

## 🔐 Error Handling & Data Validation

- **Client Side**: Formik + Yup shows instant feedback.
- **Server Side**: Joi schema validates request payloads.
- Handles invalid routes, MongoDB errors, and failed API responses gracefully.

## 🧩 Component Integration

| Component         | Purpose                          | Connected To           |
|-------------------|----------------------------------|------------------------|
| ResumeForm        | Data input                       | Updates preview + API  |
| LivePreview       | Dynamic resume preview           | Receives props         |
| TemplateSelector  | Change design dynamically        | CSS/themes             |
| ResumeExport      | Save resume as PDF               | html2pdf + preview     |
| AIHelper (opt.)   | Generate smart content via GPT   | Backend API            |

## 🧪 Code Quality & Innovation

- 💡 Modular Codebase with reusable components.
- ✅ Linted with ESLint + Prettier.
- 🧠 Innovative Features:
  - GPT-driven content suggestions
  - Real-time ATS keyword checker (planned)
  - Resume version control

## 📄 Future Enhancements

- 📊 Dashboard with resume analytics
- 🧠 Smart suggestions based on job description
- 🧾 Save multiple resume profiles
- 🌐 Localization and language support

## 🧑‍💻 Contributors

- **You!** Fork, star ⭐ and submit a pull request.
- Or contact me at `your.email@example.com` to collaborate.

## 📜 License

MIT License © 2025 [Your Name]
