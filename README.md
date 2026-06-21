🧪 TestMaster Pro

An AI-powered testing platform that helps developers automatically generate 
comprehensive test cases, improve code quality, and catch bugs early — built 
and deployed on Vercel.

🌐 **Live Demo:** https://testmaster-pro.vercel.app

---

## 🚀 Features

- 🧠 **AI-generated test cases** from your code or description
- 🔍 **Comprehensive coverage** — unit, integration and edge cases
- 🐛 **Bug detection** — AI identifies potential issues early
- ⚡ **Fast generation** — complete test suite in minutes
- 📝 **Multiple testing frameworks** — Jest, Pytest, Mocha and more
- 📱 **Fully responsive** — works on desktop and mobile

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Next.js / React | Frontend framework |
| Vercel | Deployment and hosting |
| Anthropic Claude / Gemini | AI test case generation |
| Tailwind CSS | Styling and UI |

---

## 🔄 How It Works
User Pastes Code or Describes Feature

↓

AI Analyses Code Structure & Logic

↓

Edge Cases & Scenarios Identified

↓

Comprehensive Test Suite Generated

↓

Ready to Copy into Your Project

---

## ⚙️ Setup & Installation

1. Clone the repository
```bash
git clone https://github.com/greatman-786/testmaster-pro.git
cd testmaster-pro
```

2. Install dependencies
```bash
npm install
```

3. Add environment variables
```bash
ANTHROPIC_API_KEY=your_api_key_here
```

4. Run locally
```bash
npm run dev
```

5. Open `http://localhost:3000`

---

## 📁 Project Structure
testmaster-pro/

│

├── pages/          # Next.js pages

├── components/     # Reusable UI components

├── styles/         # Tailwind CSS styles

├── lib/            # AI integration logic

└── README.md       # Project documentation

---

## 🧠 AI Integration

The AI layer powers the entire test generation process:
- **Analyses code structure** and understands the logic flow
- **Identifies edge cases** that developers commonly miss
- **Generates test cases** for happy paths, edge cases and error scenarios
- **Supports multiple frameworks** — outputs tests in Jest, Pytest, Mocha etc.
- **Explains each test case** so developers understand what is being tested
- Works with both **Anthropic Claude** and **Google Gemini**

---

## ⚡ Challenges & How I Solved Them

### 1. 🔑 API Credit Exhaustion
**Problem:** The Anthropic API key ran out of credits during testing, 
completely blocking all AI test case generation.  
**Solution:** Switched to **Google Gemini** (free tier via Google AI Studio) 
as a drop-in replacement and configured the API key properly in **Vercel 
environment variables** for secure and reliable access.

### 2. 🎯 Generating Relevant vs Generic Tests
**Problem:** Early AI outputs produced very generic test cases that didn't 
reflect the actual logic of the code being tested — making them useless 
for real projects.  
**Solution:** Refined the prompt engineering significantly — instructing the 
AI to **analyse the specific code logic** before generating tests, and to 
always include edge cases and error scenarios alongside happy path tests.

### 3. 📝 Supporting Multiple Testing Frameworks
**Problem:** Different developers use different testing frameworks — generating 
tests in only one format limited the app's usefulness significantly.  
**Solution:** Added a **framework selector** in the UI allowing users to choose 
their preferred framework (Jest, Pytest, Mocha etc.) before generation — the 
AI then outputs tests in the correct syntax for that framework.

### 4. 🚀 Vercel Deployment Issues
**Problem:** Large code inputs caused AI processing to exceed Vercel's 
serverless function timeout limits during deployment.  
**Solution:** Implemented **streaming responses** so test cases appear 
progressively as they are generated — keeping users engaged and staying 
within serverless time limits.

---

## 💡 Use Cases

- Developers automating their testing workflow
- Teams improving code quality and coverage
- Startups building reliable software faster
- Developers learning how to write better tests

---

## 🙋‍♂️ Author

**Asad** — Software Engineer  
Building AI-powered web applications for real-world use cases
