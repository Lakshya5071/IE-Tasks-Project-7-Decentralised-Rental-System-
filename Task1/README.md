
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
