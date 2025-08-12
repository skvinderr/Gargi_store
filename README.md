# Gargi Hostel Store 🛒

![Gargi Hostel Store Banner](https://ibb.co/pB5s4BTP)

**A modern, real-time e-commerce PWA (Progressive Web App) designed to bring the convenience of online shopping directly to the students of Gargi Hostel. This application provides a seamless way for students to order daily essentials, snacks, and stationery from the comfort of their rooms.**

---

## ✨ Key Features

* **🏠 Beautiful Homepage:** A stunning, animated landing page that welcomes users and explains the service.
* **📧 Secure Email & Password Authentication:** A complete user registration and login system. New users provide their name, email, and phone number to create a profile.
* **🛍️ Dynamic Product Catalog:** A clean, grid-based layout to display all available products with high-quality images.
* **🛒 Interactive Cart System:** "Add to Cart" buttons transform into `+` and `-` quantity selectors, providing a smooth and interactive shopping experience.
* **📝 Real-Time Order Management:** A dedicated **"My Orders"** section where students can:
    * View their complete order history.
    * Track the live status of their orders (Pending, Completed, Cancelled).
    * Cancel any order that is still in "Pending" status.
* **🛵 Room Number for Delivery:** A mandatory field at checkout ensures you know exactly where to deliver each order.
* **🔥 Firebase Backend:** Built on a powerful and scalable serverless backend using:
    * **Firebase Authentication** for secure user management.
    * **Firestore Database** for storing user profiles, products, and real-time order data.

---

## 🚀 Technology Stack

This project is built with a focus on simplicity, performance, and a great developer experience.

* **Frontend:**
    * **HTML5**
    * **Tailwind CSS:** For modern, responsive, and utility-first styling.
    * **Vanilla JavaScript (ES6 Modules):** For all client-side logic, keeping the application lightweight and fast.

* **Backend & Database:**
    * **Firebase:** An all-in-one backend platform providing:
        * **Firebase Authentication:** For handling user sign-up and login.
        * **Firestore:** A NoSQL, real-time database for storing all application data.

---

## 🔧 Getting Started

To get a local copy up and running, follow these simple steps.

### Prerequisites

* A modern web browser (like Chrome or Firefox).
* A code editor (like [VS Code](https://code.visualstudio.com/)).
* The [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) extension for VS Code.

### Firebase Setup

1.  **Create a Firebase Project:** Go to the [Firebase Console](https://console.firebase.google.com/) and create a new project.
2.  **Create a Web App:** Inside your project, add a new Web App to get your `firebaseConfig` keys.
3.  **Enable Authentication:** Go to **Authentication > Sign-in method** and enable the **"Email/Password"** provider.
4.  **Create Firestore Database:** Go to **Firestore Database**, create a new database, and start in **Test Mode**.

### Local Installation

1.  **Clone the Repo (or download the files):**
    ```sh
    git clone [https://github.com/your-username/gargi-hostel-store.git](https://github.com/your-username/gargi-hostel-store.git)
    ```
2.  **Rename the Files:**
    * The homepage file should be named `index.html`.
    * The main store application file should be named `store.html`.
3.  **Add your Firebase Config:**
    * Open `store.html` in your code editor.
    * Find the `firebaseConfig` variable (around line 200).
    * Replace the placeholder object with the actual `firebaseConfig` keys you got from your Firebase project.
4.  **Run with Live Server:**
    * Right-click on `index.html` in VS Code and select "Open with Live Server".

---

## 📦 Deployment

This project can be deployed in seconds using Netlify.

1.  **Sign up** for a free account at [Netlify](https://www.netlify.com/).
2.  On your Netlify dashboard, simply **drag and drop the folder** containing your `index.html` and `store.html` files.
3.  **Authorize your domain:** Don't forget to add your live Netlify URL (e.g., `your-store.netlify.app`) to the **Authorized domains** list in your Firebase Authentication settings.

---

## ⚙️ How to Manage Orders (For the Admin)

Once an order is delivered, you need to update its status.

1.  Go to your **Firestore Database** in the Firebase Console.
2.  Select the **`orders`** collection.
3.  Find the order you want to update (you can identify it by the `orderedByName` and `roomNumber` fields).
4.  Click on the order document, find the `status` field, and change its value from `"Pending"` to `"Completed"`.
5.  Click **"Update"**. The user will see this change in real-time in their "My Orders" section.

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/your-username/gargi-hostel-store/issues).

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
