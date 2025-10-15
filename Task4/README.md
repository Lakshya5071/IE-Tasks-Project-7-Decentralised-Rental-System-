
## 📖 Task 4 — “NFT-Based Event Ticketing DApp”

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
