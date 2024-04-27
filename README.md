# Live Chat App 

### Overview
The Live Chat App is a real-time messaging application that allows users to communicate with each other instantly over the internet. It provides a seamless chat experience with features such as text messaging, emoji support, and user joining and leaving indicator.
- Live Project: [Chat Now!](https://mychatapp0.azurewebsites.net/)

### Features
- **Real-time Messaging**: Messages are delivered instantly, providing a responsive chat experience.
- **Emoji Support**: Users can express themselves using a variety of emojis.
- **User Status**: Users can see a user joining or leaving.

---
### Technologies Used
- **Frontend**: HTML, CSS, JavaScript
- **Backend**: Spring Boot, Websocket
- **Deployment**: GitHub Actions, Azure

Here's a section you can add to your live chat documentation to explain WebSocket:

---

### WebSocket Integration

The live chat application utilizes the WebSocket API to enable real-time, bi-directional communication between the client's web browser and the server. This allows for instant messaging and updates without the need for continuous polling.

#### How WebSocket Works

1. **Connection Establishment**: The client initiates a WebSocket connection by sending an initial HTTP request, which is then upgraded to a WebSocket connection if the server supports it.

2. **Bi-Directional Communication**: Once the WebSocket connection is established, both the client and server can send messages to each other at any time, enabling real-time updates and notifications.

3. **Event-Driven Model**: WebSocket uses an event-driven model, where messages are sent and received asynchronously, allowing for efficient communication without the overhead of traditional HTTP requests.

4. **Persistent Connection**: Unlike traditional HTTP, which is stateless and requires a new connection for each request, WebSocket maintains a persistent connection, reducing latency and overhead.

5. **Protocol Support**: WebSocket is standardized by the IETF as RFC 6455, ensuring compatibility between different WebSocket implementations and providing a reliable communication channel.

#### Benefits of WebSocket

- **Real-Time Updates**: Enables instant messaging and updates without polling.
- **Efficient Communication**: Maintains a persistent connection for efficient, low-latency communication.
- **Scalability**: Supports large numbers of concurrent connections, making it suitable for scalable applications.
- **Reliability**: Built-in mechanisms for ensuring message delivery and connection integrity.

#### Implementation Details

The live chat application uses the WebSocket API provided by the Spring Boot framework for server-side communication. On the client side, WebSocket is implemented using JavaScript and the WebSocket API supported by modern web browsers.

---
---

### Installation
1. Clone the repository.
2. Install dependencies using Maven: `mvn install`.
3. Start the Spring Boot application: `mvn spring-boot:run`.
4. Access the app in your web browser at `http://localhost:8080`.

### Deployment
The app is automatically deployed using GitHub Actions to Azure. The deployment process is triggered on every push to the main branch.

### Usage
1. log in to the app using your name.
3. Send messages and emojis to communicate with other users in real-time.

### Future Enhancements
- **File Sharing**: Allow users to share files with each other.
- **Message History**: Provide a history of past messages for users to view.
- **Onine Status**: View the online status of other users.

### Contributing
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/my-feature`).
3. Commit your changes (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature/my-feature`).
5. Create a new Pull Request.
