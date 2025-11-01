# 🏕️ WanderLust

WanderLust is a full-stack web application inspired by Airbnb, designed to help users discover and share unique places to stay. It provides a seamless platform for users to browse, create, update, and delete property listings. The entire application is built on the MVC (Model-View-Controller) architecture and features a robust RESTful API for handling all backend operations.

---

## ✨ Key Features

-   **Dynamic CRUD Operations:** Users can easily **C**reate, **R**ead, **U**pdate, and **D**elete property listings.
-   **RESTful API:** A well-structured backend API built with Express.js to manage data efficiently.
-   **Responsive UI:** Built with Bootstrap, the user interface is fully responsive and works seamlessly on desktops, tablets, and mobile devices.
-   **Data Persistence:** MongoDB is used for storing and managing all property and user data.
-   **MVC Architecture:** A clean and organized codebase following the Model-View-Controller pattern.
-   **Image Uploads:** Users can upload images for their listings.

---

## 🛠️ Tech Stack & Tools

-   **Backend:** Node.js, Express.js
-   **Frontend:** HTML, CSS, JavaScript, EJS (Embedded JavaScript Templates), Bootstrap
-   **Database:** MongoDB with Mongoose
-   **Architecture:** MVC (Model-View-Controller)
-   **Utilities:** `method-override` for PUT/DELETE requests from forms.

---

## 🚀 Getting Started

Follow these steps to get a local copy of the project up and running for development and testing purposes.

### Prerequisites

Make sure you have the following installed on your machine:
-   [Node.js](https://nodejs.org/en/) (which includes npm)
-   [MongoDB](https://www.mongodb.com/try/download/community)

### Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/ShivamGupta-16/WanderLust.git
    ```

2.  **Navigate into the project directory:**
    ```bash
    cd WanderLust
    ```

3.  **Install the necessary npm packages:**
    ```bash
    npm install
    ```

4.  **Set up your Environment Variables:**
    Create a `.env` file in the root of your project and add your MongoDB connection string.
    ```env
    MONGO_URL="mongodb://127.0.0.1:27017/wanderlust"
    PORT=8080
    ```

5.  **Start the server:**
    ```bash
    nodemon app.js
    ```
    The application should now be running on `http://localhost:8080`.

---

## 🗺️ REST API Endpoints

The core functionality is exposed through the following RESTful API endpoints for listings:

| HTTP Verb | Path (`/listings`) | Description                     |
| :-------- | :----------------- | :------------------------------ |
| `GET`     | `/`                | Get all property listings.      |
| `GET`     | `/new`             | Show form to create a new listing. |
| `POST`    | `/`                | Create a new listing.           |
| `GET`     | `/:id`             | Get details for a single listing. |
| `GET`     | `/:id/edit`        | Show form to edit a listing.    |
| `PUT`     | `/:id`             | Update a specific listing.      |
| `DELETE`  | `/:id`             | Delete a specific listing.      |

---

## 🔮 Future Enhancements

Here are some features planned for future development:
-   [ ] **User Authentication:** Add user signup, login, and profile management.
-   [ ] **Reviews and Ratings:** Allow users to leave reviews and ratings on listings.
-   [ ] **Interactive Map View:** Integrate a map to show property locations.
-   [ ] **Search and Filter:** Implement advanced search and filtering options for listings.
