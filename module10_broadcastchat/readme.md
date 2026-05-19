#  2.1: Original code, and how it runs

![alt text](image.png)

Explanation: Start the server using cargo run --bin server, then launch multiple clients across separate terminals with cargo run --bin client. When any client sends a message, the server instantly broadcasts it to all other active connections. This process relies on asynchronous execution, allowing the server to manage all client traffic concurrently without blocking.

