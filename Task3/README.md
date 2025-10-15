
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
 