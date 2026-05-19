#  2.1: Original code, and how it runs

![alt text](image.png)

Explanation: Start the server using cargo run --bin server, then launch multiple clients across separate terminals with cargo run --bin client. When any client sends a message, the server instantly broadcasts it to all other active connections. This process relies on asynchronous execution, allowing the server to manage all client traffic concurrently without blocking.

## 2.2 Modifying Port

![alt text](image-1.png)

The port was changed from 2000 to 8080 in both server.rs and client.rs. The files are modified because WebSocket is a connection-based protocol. Both Server and Client file must use same port. ws:// prefix indicates it is using the WebSocket protocol. And after that the server manage all client traffic concurrently without any blocking.