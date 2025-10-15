
# 🧠 Task 5: The AI Study Buddy

 ### **Marks:** 50
 ### **Frontend**  React.js , 
 ### **Backend:** Node.js (Express) 
 ### **AI:** Any public LLM API (e.g., OpenAI, Gemini, Claude)


## 🎯 Project Goal

Your goal is to build a **robust, interactive, and user-friendly AI-powered study tool**.  
This application will transform a **large block of unstructured text** (like class notes or an article) into a **structured, multi-format learning experience**.

The core challenge lies in designing a **single, complex AI prompt** and building a **highly interactive React frontend** to visualize and manage the structured data generated.

---

## 🧩 Detailed Feature Requirements

### 🖋️ The Input Interface

- A clean, single-view layout.
- The **left side** should feature a **large, resizable textarea** for users to paste their text.
- The textarea should include a placeholder:
  > “Paste your article, lecture notes, or any block of text here...”
- A single, **prominent button** labeled **“Generate Study Aids.”**
- Once clicked, the button should:
  - Show a **loading state** (like a spinner).
  - Become **disabled** until the AI response is received or an error occurs.

---

### 🤖 The AI Generation & Data Transformation

- The backend should receive the raw text and make a **single API call** to an LLM.
- Your **prompt engineering** is critical:
  - The prompt must instruct the AI to analyze the text and return a **single, valid JSON object**.
  - The JSON must include **three data types** — summary, flashcards, and quiz — in one response.

---

### 📚 The Interactive Study Dashboard

This will be a **tabbed component** on the right side of the screen with three tabs:

#### 📝 Summary Tab
- Displays the **AI-generated summary** in a clean, readable format.

#### 🎴 Flashcards Tab
- Displays **only one flashcard at a time**.
- Each flashcard initially shows the **term**.
- When clicked, it **flips** to show the **definition** (using a CSS transform animation).
- Clicking again flips it back.
- Include **“Previous”** and **“Next”** buttons to navigate.
- Show a progress indicator like:
  > “Card 5 of 18”

#### 🧩 Quiz Tab
- Displays **one multiple-choice question** at a time.
- Each option is clickable.
- Once an option is selected:
  - All buttons become **disabled**.
  - The chosen option turns **green if correct** or **red if incorrect**.
  - If incorrect, the **correct answer** is highlighted in green.
- A **“Next Question”** button appears **after** answering the current one.
- After the final question, show a **results screen**:
  > “You scored 7 out of 10!”

---


## 🚀 Bonus Challenges (Optional)

* Add a **“Copy to Clipboard”** button for the summary.
* Display a **detailed result breakdown** showing which quiz questions were answered incorrectly.
* Add an option to **shuffle flashcards** in random order.

---

## 📦 Submission Checklist

* A **public GitHub repository** with:

  * `/client` and `/server` folders.
  * A `README.md` file containing:

    * Clear, step-by-step setup instructions.
    * A detailed section describing your **prompt engineering strategy** for generating clean JSON output.

---

## 🧠 Evaluation Focus

Your submission will be judged on the following:

1. **Prompt Engineering** —
   How effectively your prompt ensures the AI returns accurate, structured JSON every time.

2. **React State Management** —
   The quality of logic handling for flashcard flipping, quiz progression, and score calculation.

3. **UI/UX & Robustness** —
   Clarity, responsiveness, and resilience of your interface — including handling loading and error states gracefully.

