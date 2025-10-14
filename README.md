# 🚀 Web3 & AI Project Tasks — Choose Your Task Wisely

This mainly consists of **5 tasks**, each designed to challenge you at different difficulty levels — from **beginner-friendly** Solidity practice to **advanced full-stack AI + blockchain integrations**.

Your mission is to **select one task** that best matches your current skill level, complete it thoroughly, and submit it as a **public GitHub repository**.  
> 💡 Remember: One complete, polished submission is always better than multiple half-finished attempts.

---

## 🧭 Choosing the Right Task Level

Each task has been crafted for a specific experience tier.  
Use the guide below to pick your ideal project:

### 🟢 Beginner Level — Solidity & Web Fundamentals

**Recommended for:**  
- Students with **no prior experience** in web development or Solidity.

**Focus:**  
- For Solidity beginners: Core smart contract logic, Solidity syntax, events, mappings, and basic blockchain interaction using **Remix IDE**.  
- For Web beginners: Basic frontend development skills, component rendering, state handling, and simple interactivity using **React/Tailwind CSS**.

**Goal:**  
- Solidity learners: Understand how decentralized applications work at the **contract layer**, without worrying about frontend or deployment tools.  
- Web learners: Learn how to **build interactive UI components, handle user inputs, and display dynamic content**, preparing for future integration with blockchain.


### 🟡 Intermediate Level — Web + Blockchain Integration
**Recommended for:**  
- Developers who have a **basic idea of web development** and are interested in exploring **how frontends connect with smart contracts**.

**Focus:**  
- Hands-on experience with **Hardhat, MetaMask, and IPFS**, while building meaningful decentralized applications.

**Goal:**  
- Bridge the gap between **Solidity and Web3 UI**, understanding contract deployment, data retrieval, and interaction flows.

### 🔴 Advanced Level — Full-Stack Web3 + AI Systems
**Recommended for:**  
- Students who are comfortable with **both Web and Blockchain**, and want to explore **AI-powered DApps** or complex full-stack systems.

**Focus:**  
- End-to-end systems combining **AI models, decentralized storage, and blockchain smart contracts**.  
- These projects demand **good problem-solving**, API handling, and UI/UX design.

**Goal:**  
- Showcase your ability to build a **production-level Web3 + AI application**.


## ✅ Submission Guidelines

1. Choose **only one task** based on your skill level. If you have enough time you can also attempt other tasks as well.
   Completing one full project demonstrates better understanding than starting multiple.

2. Ensure your **GitHub repository is public**.  
   - Include clear commit history.  
   - Add a detailed `README.md` explaining setup, functionality, and technologies used.

3. **Submit your completed project here:**  
[**Google Form Link**](https://docs.google.com/forms/d/e/1FAIpQLSfi-VRmObHL9TBfbqnmlPW57AhyQo7ObyNGe20FjXmWPTz1hw/viewform?usp=header)

## 🧩 Final Advice

- Read the task description thoroughly before starting.  
- Plan your approach — architecture, data flow, and component structure.  
- Prioritize **completeness and clarity** over adding unnecessary features.  

> 💬 “Focus on building something that works beautifully — not just something that barely runs.”
> - For any doubts, feel free to contact us,  
  > M.Lakshya - 9019840753  
  > Anirudh S - 7349063909  
  > Naman - 9257857284

---

## Beginner

## 🧠 Task 1 — Decentralized Feedback Vault

### 🎯 Marks: 20
### 🧰 Tools: Remix IDE only
### 🏗️ Focus: Solidity fundamentals — structs, mappings, modifiers, events, require/assert

---

### 📌 Objective

Design and deploy a **Decentralized Feedback Vault** smart contract where users can **submit, view, and rate feedback** directly on the blockchain. This project will test your understanding of **Solidity data structures, function visibility, modifiers, mappings, and smart contract logic design**.

The contract should allow **users to interact with the system anonymously**, while also ensuring **integrity, validation, and organization** of submitted data.

---

### ⚙️ Requirements

1. **Feedback Submission**

   * Any wallet address should be able to submit feedback in the stored data.
   * Each feedback should be stored with a unique identifier.

2. **Feedback Rating System**

   * Other users should be able to **upvote or downvote** existing feedbacks.
   * Prevent users from rating the same feedback multiple times.

3. **Validation and Modifiers**

   * Include modifiers to restrict misuse — for example, a modifier that prevents empty feedback submissions or repeated ratings.
   * Use `require`, `assert`, or `revert` statements to enforce logical checks.

4. **Admin**

   * The contract deployer can act as an **admin** who can:

     * Archive or delete inappropriate feedback.
     * View total feedback statistics.

5. **Events and Mappings**

   * Use events for logging submissions, ratings, and admin actions.
   * Use mappings efficiently to track and manage feedbacks, votes, and users.

---

### 🚀 Deliverables

* A deployed smart contract on **Remix IDE**.
* The final `.sol` file exported from Remix.
* A short demo (optional but recommended) showing:

  * Feedback submission
  * Upvoting/downvoting
  * Admin actions

---

### 🧩 Bonus (Extra Marks)

You may add **optional advanced features** such as:

* Feedback categories or tags (e.g., “UI”, “Performance”, “Features”)
* Timestamps for each submission
* Weighted reputation system where users with more contributions have higher rating power

---

### 💡 Tip

Keep your contract **modular, readable, and test-driven**. Use **clear naming conventions**, **proper comments**, and **event logs** to make your submission stand out.

---

### ✅ Evaluation Criteria — What You’ll Be Judged On

1. **Code Logic & Solidity Fundamentals** — Efficient use of structs, mappings, modifiers, and validation.
2. **Clean Design & Readability** — Proper function naming, comments, and modular structure.
3. **Functionality & Creativity** — Smooth execution of feedback flow and any innovative bonus features.

---

## 🏦 Task 2 — Decentralized Peer-to-Peer Micro-Lending

 ### **Marks:** 25
### **Tools:** Remix IDE
### **Focus:** Solidity fundamentals, payable ETH transfers, multi-user interactions, state management, events

---

### 🎯 Objective

Create a **blockchain-based P2P micro-lending platform** where:

* Users can request loans in ETH.
* Multiple lenders can contribute **partial amounts** to the same loan.
* Borrowers repay each lender **individually** with interest.
* Admin monitors platform statistics but **does not control funds**.

---

### ⚙️ Requirements & Features

1. **Loan Requests**

   * Borrowers can request a loan with a specified ETH amount and interest rate.
   * The platform should track total requested, remaining unfunded amount, and status of each loan.
   * All requests should be recorded on-chain with events for transparency.

2. **Partial Funding by Multiple Lenders**

   * Lenders can fund loans partially.
   * Each lender’s contribution and corresponding interest is tracked individually.
   * The remaining amount of the loan is updated as funding progresses.

3. **Loan Repayment**

   * Borrowers repay each lender separately, including the agreed interest.
   * On repayment, lender balances are updated and events are emitted.

4. **Loan History and Status**

   * Borrowers can view all their loans and repayment progress.
   * Lenders can view their funded loans and pending repayments.
   * Admin can view overall platform statistics including total loans and repayments.

5. **Validation & Security**

   * Prevent zero-value loans and funding.
   * Ensure borrowers cannot overpay or funders cannot overfund.
   * Maintain integrity of partial funding for multiple lenders.

---

### 💡 Optional Bonus Features (+5 Marks)

* Allow borrowers to **prepay selected lenders** to reduce interest.
* Implement **tiered interest rates** to incentivize early lenders.

---

### ✅ Evaluation Criteria — What You’ll Be Judged On

1. **Smart Contract Logic & ETH Handling** — Secure use of `payable`, transfers, and balance tracking.
2. **Multi-User Workflow** — Smooth borrower–lender interactions and loan lifecycle handling.
3. **Code Structure & Innovation** — Readability, validation, and any creative bonus features.

---

## 🎯 Task 3: Property Dashboard (Single Combined Frontend Task) 
 
 ### **Marks:** 25
### **Tools:** React.js/Javascript

Build a **Property Dashboard** — a single, polished frontend application that implements the **core UI surface** for the **Blockchain-based Rental Project**. This task focuses on building a feature-rich, interactive, and user-friendly dashboard with search, filters, persistence, and property management features — all handled locally or with a mock API.

---

## 🧠 Objectives

1. **Property Listing**
   - Render a paginated property list in a **card or grid layout** from local data.

2. **Search & Filters**
   - Implement **debounced text search**.
   - Add **composed filters** — city, price range, property type, bedrooms.
   - Ensure all filters work seamlessly with pagination.

3. **Property Details View**
   - Provide a **modal or route-based detail view** for each property.
   - Include:
     - Image carousel
     - Full description
     - Amenities list
     - Landlord information

4. **Request/Booking Form**
   - Build a form with **client-side validation** and **local persistence** (simulate submitting requests).
   - Ensure form state and feedback are handled gracefully.

5. **Wishlist / Favorites**
   - Allow users to add/remove properties from a **wishlist**.
   - Persist wishlist locally and sync across all views.

6. **CSV Import**
   - Support importing new property data via CSV.
   - Parse, validate, preview, and merge imported rows into the dataset.

7. **Preference-Based Matching**
   - Implement a **simple ranking UI** that matches user preferences with available properties.
   - Clearly explain **“why it matched”** for transparency.

---

## ⚙️ Requirements

1. **Tech Stack & Setup**
   - Use **React (Vite)** and **Tailwind CSS**.
   - Optionally use **json-server** to simulate a mock REST API.

2. **Mock Data & Persistence**
   - Use `properties.json` as the **canonical dataset**.
   - Enable **CSV import** support.
   - Persist **wishlist** and **booking requests** in `localStorage` (simulate transaction logs).

3. **Core Functionalities**
   - Paginated property list  
   - Debounced search + composed filters  
   - Property detail (modal/route) with carousel  
   - Request/booking form  
   - Wishlist page  
   - CSV import support  
   - Preference-based ranking interface

4. **Accessibility & Responsiveness**
   - Fully responsive layout for **mobile, tablet, and desktop**.
   - Include **keyboard navigation** and **ARIA attributes** where necessary.
   - Resolve major **Lighthouse** or **axe accessibility issues**.

5. **Quality & UX**
   - Reusable, modular React components.
   - Clear **error handling** and **loading/skeleton states**.
   - Include subtle **animations** or **visual feedback** for user actions.

6. **Developer Practices**
   - Maintain **meaningful commit history**.
   - Submit via a **single PR/branch**.
   - Include a **README** with setup, data format, and run instructions.

---

## 📦 Deliverables

1. **GitHub Repository**
   - Contains the full app with a clear and consistent commit history.

2. **README.md**
   - Includes:
     - Setup and installation steps.
     - Instructions for running locally.
     - `json-server` setup guide (if applicable).
     - Information about `properties.json` and CSV import.
     - How to view saved requests and wishlist.

3. **Sample Data**
   - `properties.json` — canonical dataset.  
   - `sample-properties.csv` — with headers and example rows.

4. **Demo Evidence**
   - 2–3 screenshots (e.g., property list, detail modal, CSV import, wishlist).  
   - OR a short **1–2 minute demo video** showcasing the workflow.

---

## 🧮 Evaluation Criteria

Your submission will be judged on the following three key aspects:

1. **Functionality & Completeness** —  
   How well the required features (pagination, filters, modals, forms, CSV import, etc.) are implemented and interconnected.

2. **UI/UX Quality** —  
   Smoothness of interactions, visual consistency, accessibility, and responsiveness across devices.

3. **Code Quality & Developer Practices** —  
   Code organization, reusability, component design, commit hygiene, and clarity of documentation.

---

##Intermediate:

## 📖 Task 3 — “NFT-Based Event Ticketing DApp”

 ### **Marks:** 50
 ### **Tools:** Hardhat, MetaMask, frontend (React/HTML/JS), ERC721,
 ### **Focus:** NFTs, smart contracts, Hardhat deployment, frontend integration

---

### 🎯 Objective

Create a **mini NFT ticketing platform** where:

* Event organizers can **mint NFT tickets** for events.
* Each ticket NFT stores **metadata**: seat number, event date, category.
* Users can **purchase tickets** using ETH or ERC20 tokens.
* Users can **transfer or resell tickets** securely.
* Frontend displays ticket ownership, event details, and allows transfers.

This task must be done by:

1. **Setting up Hardhat** in your local environment.
2. **Deploying the NFT marketplace smart contract** using Hardhat to a local or test network.
3. **Connecting the frontend** to interact with the deployed contract via MetaMask.
4. Optionally, store ticket images or QR codes on **IPFS**.

---

### ⚙️ Requirements & Features

1. **NFT Minting by Event Organizers**

   * Only authorized organizers can mint tickets.
   * Metadata includes **seat info, event date, ticket category**.

2. **Ticket Purchase**

   * Users can buy tickets using ETH or ERC20 tokens.
   * Ownership is updated immediately on purchase.

3. **Ticket Transfer / Resale**

   * Owners can transfer tickets securely.
   * Optional: enforce rules like **no resale above max price**.

4. **Frontend Display**

   * Show all minted tickets with **ownership and event details**.
   * Organizer dashboard to view ticket sales.

5. **Validation**

   * Prevent minting without proper metadata.
   * Ensure only organizers can mint.
   * Check sufficient payment before completing purchase.

---

### 💡 Optional Bonus Features (+5 Marks)

* Store **ticket images or QR codes on IPFS**.
* Implement **dynamic pricing**: early-bird, VIP, or last-minute discounts.
* Add **ticket perks**: backstage passes, merchandise coupons linked via metadata.

---

### 📦 Deliverables

1. **Smart Contract**

   * Deployed via Hardhat on a local or test network.
   * Includes minting, ownership transfer, and metadata logic.

2. **Frontend Application**

   * Connected with MetaMask for buying, transferring, and displaying tickets.
   * Includes organizer dashboard and event details section.

3. **Optional IPFS Integration**

   * Store ticket visuals or QR codes on IPFS.
   * Link IPFS hash (CID) in NFT metadata.

4. **README / Documentation**

   * Setup instructions, commands for Hardhat and frontend.
   * Explanation of contract functions and user flow.
   * Demo(1 or 2 min) would be appreciated.


---

### 🧾 Evaluation Criteria — *What You’ll Be Judged On*

1. **Functionality & Blockchain Logic:**
   Whether the NFT minting, purchasing, and ownership transfer work correctly and securely on-chain.

2. **Frontend Integration & User Interaction:**
   How well the frontend communicates with the blockchain through MetaMask and provides a smooth, intuitive experience.

3. **Smart Contract Quality**
   Is the Solidity code well-structured, secure, and efficient? Are access controls (e.g., only organizers can mint) properly implemented? 


# 🧠 Task 4: The AI Study Buddy

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


## Advanced: 


## 📖 Task 5 — “Blockchain Story Registry with IPFS”

 ### **Marks:** 100
 ### **Tools:** Hardhat, MetaMask, frontend (React/HTML/JS), LLM/Gemini API, IPFS
 ### **Focus:** Solidity, Hardhat deployment, IPFS integration, frontend connection, LLM API usage

---

### 🎯 Objective

Create a **fun decentralized application** where:

* Users can **generate a custom story** using an AI (LLM/Gemini API).
* The generated story is **stored on IPFS**, and only the **CID is stored on the blockchain** under the user’s address.
* Users can view **all stories registered**, fetch content from IPFS, and see the creator.
* Frontend displays the story by **retrieving content from IPFS using the stored CID**.

This project must be done by:

1. **Setting up Hardhat** in the local environment.
2. **Deploying the smart contract** using Hardhat to a local or test network.
3. **Integrating IPFS** to store story content.
4. **Connecting a frontend** to the deployed contract using **MetaMask** to fetch CIDs and display content.

This ensures students learn **full-stack Web3 workflows with decentralized storage**.

---

### ⚙️ Requirements & Features

1. **Story Generation**

   * User describes their thought/idea/emotion as input.
   * LLM API generates a short, creative story based on the input.

2. **Story Storage & Registration**

   * Upload the generated story to **IPFS** to get the **CID**.
   * Smart contract stores **only the CID** along with the creator’s address.
   * Emit an event when a story CID is registered.

3. **Frontend Display**

   * Frontend retrieves all CIDs from the contract.
   * Fetch story content from IPFS using the CID.
   * Display stories with **creator addresses** and optionally filter by creator.

4. **Validation**

   * Prevent empty story submissions.
   * Limit story size if necessary (to prevent large IPFS uploads).

---

### 💡 Optional Bonus Features (+5 Marks)

* Generate a **fun illustration** for each story using an AI image API and store it on IPFS, linking the CID in the smart contract.

---

### 📦 Deliverables

1. **Smart Contract**

   * Deployed via Hardhat on a local or test network.
   * Contains logic for storing CIDs and emitting registration events.

2. **Frontend Application**

   * Integrated with MetaMask to interact with the deployed contract.
   * Allows users to submit prompts, generate stories via LLM, and fetch from IPFS.

3. **IPFS Integration**

   * Store story content (and optionally images) on IPFS.
   * Only CIDs stored on-chain for lightweight and efficient storage.

4. **README / Documentation**

   * Clear setup steps for local environment and deployment.
   * Commands for Hardhat, IPFS upload, and running the frontend.

---

### 🧾 Evaluation Criteria — *What You’ll Be Judged On*

1. **End-to-End Functionality:**
   How smoothly the flow works — from AI-generated story creation, IPFS upload, blockchain registration, to frontend display.

2. **Technical Implementation & Code Quality:**
   Solidity contract correctness, event handling, IPFS integration, and efficient frontend-backend connection.
