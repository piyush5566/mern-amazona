# MERN AMAZONA

![amazona](/frontend/public/images/amazona.jpg)

## Table of Contents
- [Demo Website](#demo-website)
- [Project Description](#project-description)
- [Run Locally](#run-locally)
  - [Prerequisites](#prerequisites)
  - [Steps](#steps)
- [Contributing](#contributing)
- [Troubleshooting](#troubleshooting)
- [License](#license)

## Demo Website

- 👉 Render : [https://amazona.onrender.com](https://amazona.onrender.com)

## Project Description

MERN Amazona is an e-commerce platform built using the MERN stack (MongoDB, Express.js, React, and Node.js). It supports user authentication, product browsing, and an admin interface for managing users and products.

## Run Locally

### Prerequisites

- Node.js
- MongoDB (local or Atlas Cloud)

### Steps

1. **Clone repo**
    ```sh
    $ git clone git@github.com:piyush5566/mern-amazona.git
    $ cd mern-amazona
    ```

2. **Create .env File**
    - Duplicate `.env.example` in the `backend` folder and rename it to `.env`.

3. **Setup MongoDB**
    - **Local MongoDB**
      - Install it from [here](https://www.mongodb.com/try/download/community).
      - In `.env` file update `MONGODB_URI=mongodb://localhost/amazona`.
    - **Atlas Cloud MongoDB**
      - Create a database at [https://cloud.mongodb.com](https://cloud.mongodb.com).
      - In `.env` file update `MONGODB_URI=mongodb+srv://your-db-connection`.

4. **Run Backend**
    ```sh
    $ cd backend
    $ npm install
    $ npm start
    ```

5. **Run Frontend**
    ```sh
    # open new terminal
    $ cd frontend
    $ npm install
    $ npm start
    ```

6. **Seed Users and Products**
    - Run this on browser: `http://localhost:5000/api/seed`
    - It returns admin email and password and 6 sample products.

7. **Admin Login**
    - Run `http://localhost:3000/signin`.
    - Enter admin email and password and click signin.

## Contributing

Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes.
4. Commit your changes (`git commit -am 'Add new feature'`).
5. Push to the branch (`git push origin feature-branch`).
6. Create a new Pull Request.

## Troubleshooting

- Ensure MongoDB is running if you encounter connection issues.
- Check the console for any error messages and consult the documentation for solutions.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
