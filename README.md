# Join Frontend (jurin1-join_frontend)

This repository contains the frontend code for the Join project, a Kanban project management tool. This frontend is built using Vanilla JavaScript, HTML, and CSS, and is designed to work in conjunction with the [Join Backend](https://github.com/jurin1/join_backend) (which is a Django backend).

## Prerequisites

Before you begin, ensure you have the following installed:

*   **Node.js and npm (or yarn):**  Required for installing frontend dependencies and generating documentation. You can download Node.js from [https://nodejs.org/](https://nodejs.org/).
*   **A web browser:**  To run and view the frontend application (Chrome, Firefox, Safari, etc.).
*   **[Join Backend](https://github.com/jurin1/join_backend):**  **Crucially, this frontend is designed to communicate with the Join Backend. You need to have the backend project set up and running for the frontend to function correctly with full features.**

## Installation

1.  **Clone the repository:**

    ```bash
    git clone <repository-url-for-jurin1-join_frontend>
    cd jurin1-join_frontend
    ```

2.  **Install dependencies:**

    This project uses `npm` (Node Package Manager) to manage frontend dependencies. If you prefer `yarn`, you can use that as well.

    Using npm:

    ```bash
    npm install
    ```

    Or using yarn:

    ```bash
    yarn install
    ```
    This command will install the `jsdoc` dependency, which is used for generating documentation.

## Running the Frontend

The Join Frontend is a client-side application. You can run it by simply opening the `index.html` file in your web browser.

1.  **Open `index.html`:** Navigate to the project directory (`jurin1-join_frontend`) and open the `index.html` file in your preferred web browser (e.g., by double-clicking the file or right-clicking and selecting "Open with...").

    This will load the login page of the Join application.

**Important:** For the frontend to work correctly with all features (like user authentication, data persistence, etc.), the **Join Backend must be running and accessible**.

*   **Ensure the Join Backend is set up and running.**  Refer to the documentation of the (https://github.com/jurin1/join_backend) for instructions on how to install and run the backend.
*   **Verify Backend URL:** The frontend is currently configured to communicate with a backend API at `http://127.0.0.1:8000/api/` (see `scripts/storage.js`). If your backend is running on a different URL or port, you will need to update this within the `scripts/storage.js` file.

## Documentation

This project includes JSDoc documentation for the JavaScript files. To generate the documentation:

1.  **Run the documentation generation script:**

    ```bash
    npm run generate-docs
    ```

2.  **View Documentation:** After running the script, the documentation will be generated in the `docs/` directory. Open `docs/index.html` in your browser to view the documentation.

## Directory Structure

*   **`assets/`**: Contains static assets like images, SVG icons, and HTML templates for different sections of the application.
*   **`css/`**: Holds all the CSS stylesheets for styling the application.
*   **`scripts/`**: Contains all JavaScript files for the frontend logic and functionality.
*   **`docs/`**:  Where the generated JSDoc documentation is located after running `npm run generate-docs`.
*   **`fonts/`**: Contains font files used in the project.
*   **`mediaquerys/`**:  CSS files for responsive design, handling different screen sizes.
*   **`index.html`**: The main entry point for the frontend application, serving as the login page.
*   **`package.json`**:  Defines project dependencies and scripts for development.


For any questions or issues, please refer to the project maintainers or create an issue in the repository.
