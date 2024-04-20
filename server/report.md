Here is step-by-step instructions to setup the backend: 

### Step 1: Install Dependencies
Make sure you have Node.js installed on your system. Then, navigate to your project directory in the terminal and run the following command to install the required dependencies:

```bash
npm install
```

### Step 2: Configure Environment Variables
Create a `.env` file in the root directory of your project and add the following environment variables:

```
MONGO_URI=your_mongodb_connection_string
PORT=your_preferred_port_number
```
Replace `your_mongodb_connection_string` with the connection string of your MongoDB database, and `your_preferred_port_number` with the port number you want the server to run on.

### Step 3: Database Setup
Ensure your MongoDB database is running. The `DBconfig.js` file should handle the connection to the database automatically when the server starts.

### Step 4: Run the Server
You can start the server by running the following command:

```bash
npm run dev
```

This command will execute the `server.js` file, which contains the Express application setup and routes.

### Step 5: Test the Endpoints
Once the server is running, you can test the endpoints using tools like Postman or by accessing them through your browser.

- Access the homepage at `http://localhost:PORT/`.
- Access the API endpoint to retrieve all recipes at `http://localhost:PORT/api/recipes`.
- Access other API endpoints as described in your `server.js` file, such as searching for recipes by name or ingredients.

### Step 6: Additional Configuration (Optional)
You can further customize the application according to your requirements. For example, you can modify the routes, add authentication, or enhance error handling.

That's it! Your backend setup is complete, and you should now have a functional backend server for your project.