# Internet CHat

This is a simple Java-based chat application that allows multiple clients to connect to a central server and exchange messages. This README provides instructions on how to set up and run the chat application.

## Prerequisites
- Java Development Kit (JDK) installed on your system
- Eclipse IDE (or any other Java IDE of your choice)

## File Structure
- `ChatServer.java`: Contains the server-side logic for handling client connections and message broadcasting.
- `ChatClient.java`: Represents the client-side logic for connecting to the server and sending/receiving messages.
- `UserThread.java`: Manages individual client connections on the server side.
- `ReadThread.java`: Responsible for reading server input and displaying messages to clients.
- `WriteThread.java`: Handles user input and sends messages from clients to the server.

## How to Run the Chat Application

1. **Clone the Repository:**
   - Clone the repository to your local machine using Git:
     ```
     git clone <repository_url>
     ```

2. **Import the Project into Eclipse:**
   - Open Eclipse IDE.
   - Click on "File" -> "Import" -> "Existing Projects into Workspace."
   - Select the project folder where you cloned the repository.
   - Click "Finish" to import the project into Eclipse.

3. **Run the Chat Server:**
   - Open the `ChatServer` class in Eclipse.
   - Right-click on the file and select "Run As" -> "Java Application."
   - The server will start running and listen for client connections.

4. **Run Chat Clients:**
   - Open the `ChatClient` class in Eclipse.
   - Right-click on the file and select "Run As" -> "Java Application."
   - Enter the server's hostname or IP address and the port number (e.g., 5000) when prompted.
   - Multiple clients can be run simultaneously by repeating the above step.

5. **Interact with the Chat Application:**
   - Once the clients are connected, they can exchange messages with each other through the server.
   - Type messages in the client's console and press Enter to send them to the server.
   - All connected clients will receive messages broadcasted by the server.

6. **Terminating the Chat Application:**
   - To disconnect a client, type "bye" and press Enter.
   - The client will disconnect from the server.
   - To stop the server, simply terminate the server program in Eclipse.

## Important Notes
- Ensure that the port number used in the `ChatServer` and `ChatClient` classes matches and is not blocked by your firewall.
- Properly handle exceptions, especially in real-world scenarios, to enhance the application's robustness.
- This chat application does not include security features like encryption or authentication. It is meant for educational purposes and should not be used in production environments without implementing necessary security measures.
