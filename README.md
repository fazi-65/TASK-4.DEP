# TASK-4.DEP
To compile and run the multi-threaded web server code provided, follow these steps:

Step 1: Save the Code
Open your favorite text editor or IDE.
Copy the complete C++ code provided in the previous response.
Save the file as web_server.cpp.
Step 2: Prepare HTML Files
Create a directory named www (or any name you prefer) in the same location where web_server.cpp is saved.
Inside this directory, create an index.html file with some sample HTML content. For example:
html


Copy
<!-- www/index.html -->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Welcome to My Web Server</title>
</head>
<body>
    <h1>Hello, World!</h1>
    <p>This is a simple multi-threaded web server.</p>
</body>
</html>
Step 3: Compile the Code
Open a terminal (or command prompt) and navigate to the directory where web_server.cpp is saved. Use the following command to compile the code:

bash


Copy
g++ -o web_server web_server.cpp -pthread
-o web_server specifies the output executable name.
-pthread links the pthread library, which is necessary for multi-threading.
Step 4: Run the Server
Once the code is compiled successfully, you can run the server with the following command:

bash


Copy
./web_server
Step 5: Access the Server
Open a web browser.
Navigate to http://localhost:8080/. You should see the content of index.html displayed in your browser.
You can also try accessing other files by entering their paths in the URL (e.g., http://localhost:8080/about.html), but make sure those files exist in the same directory as index.html.
Step 6: Stop the Server
To stop the server, you can press Ctrl + C in the terminal where the server is running.

Additional Notes
Ensure that you have the necessary permissions to bind to the specified port (8080). If you encounter permission issues, you can try using a different port number (e.g., 8081).
If you want to serve additional HTML files, simply create them in the same directory where index.html is located, and you can access them using their respective paths.
