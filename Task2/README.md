
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
