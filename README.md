# PizzaStore Project

Welcome to the **PizzaStore** project! This is a full-stack application designed to manage a pizza store, featuring a React-based frontend (`PizzaClient`) and a .NET backend (`PizzaStore`). Below, you'll find an overview of the project structure, features, setup instructions, and technologies used.

---

## Project Structure

-   **PizzaClient**: The frontend directory containing React components, pages, services, and configuration files.
-   **PizzaStore**: The backend directory containing controllers, models, data access layers, and the main application entry point.

---

## Features

### Frontend

-   User-friendly interface for managing pizzas, orders, and customers.
-   Built with **React** and styled using **Material-UI**.
-   Communicates with the backend via **RESTful APIs**.

### Backend

-   Robust backend built with **.NET 8.0**.
-   Uses **Entity Framework Core** for database operations.
-   Provides RESTful APIs for managing pizzas, orders, and customers.

---

## Prerequisites

Before you begin, ensure you have the following installed:

-   **Node.js** and **npm** (for the frontend).
-   **.NET SDK 8.0** (for the backend).

---

## Setup Instructions

1. Clone the repository:

    ```bash
    git clone https://github.com/romeoantony/PizzaStore.git
    cd PizzaStore
    ```

2. Install frontend dependencies:

    ```bash
    cd PizzaClient
    npm install
    ```

3. Restore backend dependencies:

    ```bash
    cd ../PizzaStore
    dotnet restore
    ```

---

## Running the Application

### Backend

1. Apply migrations and seed the database:

    ```bash
    dotnet ef database update
    ```

2. Run the backend:

    ```bash
    dotnet run
    ```

### Frontend

1. Start the development server:

    ```bash
    cd ../PizzaClient
    npm run dev
    ```

2. Access the application at [http://localhost:5173](http://localhost:5173).

---

## Technologies Used

-   **Frontend**: React, Material-UI, Vite.
-   **Backend**: .NET 8.0, Entity Framework Core.
-   **Database**: SQLite.

---

## API Endpoints

### Pizza Management

-   `GET /pizzas`: Retrieves all pizzas.
-   `POST /pizzas`: Adds a new pizza.
-   `PUT /pizzas/{id}`: Updates an existing pizza.
-   `DELETE /pizzas/{id}`: Deletes a pizza.

---

Enjoy building and managing your pizza store with **PizzaStore**!
