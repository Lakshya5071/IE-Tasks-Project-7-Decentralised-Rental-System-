

## 📖 Task 6 — “Blockchain Story Registry with IPFS”

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
