# Simple HTTP Server in C 🚀 🚀🚀

This is a basic implementation of an HTTP server in C. The server listens on a specified port (in this case, 8080) and responds with a simple HTTP/1.1 200 OK response along with a cure message.

## Prerequisites

Make sure you have a C compiler either gnu/gcc or clang installed on your system. I am using standard C libraries and should work on most systems.

## How to Run

- Compile the server:

   ```bash
   gcc server.c -o server
    ```

- Run the server:
    ```bash
    ./server
    ```


# Explanation ℹ️
- **server.c:** This is the main C file containing the server code.

- **SERVER_PORT:** The port on which the server listens for incoming connections.

- **BUFFER_SIZE:** The size of the buffer used to store incoming data.

- **handle_request:** A function that handles the incoming client request. In this case, it sends a simple HTTP response.

- **main:** The main function where the server socket is created, bound to a specific port, and listens for incoming connections.


# How It Works 🕹️🕹️
- The server creates a socket using socket(AF_INET, SOCK_STREAM, 0).

- The server sets up the server address structure.

- It binds the socket to the server address using bind.

- The server listens for incoming connections using listen.

- In the main loop, the server accepts incoming connections using accept.

- It receives data from the client using recv.

- The handle_request function is called to process the client's request.

- The server sends a response to the client.

- The connection is closed using close.


# Documentation/Sources I Referred 📚 📚 📚 

1. **Blog:** [How I Built a Simple HTTP Server From Scratch Using C](https://dev.to/jeffreythecoder/how-i-built-a-simple-http-server-from-scratch-using-c-739)
   ![Blog Preview](https://res.cloudinary.com/practicaldev/image/fetch/s--KaDpzHZY--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_800/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/3wokm1drbw00ax60o4ns.png)

2. **Stack Overflow Discussion:** [Build a Simple HTTP Server in C](https://stackoverflow.com/questions/176409/build-a-simple-http-server-in-c)
![Stack Overflow Preview](https://trungams.github.io/assets/img/socket-programming-tcp.png)

3. **YouTube Tutorial:** [Building a Simple HTTP Server in C](https://www.youtube.com/watch?v=cEH_ipqHbUw&pp=ygUQaHR0cCBzZXJ2ZXIgaW4gYw%3D%3D)
![YouTube Tutorial Preview](https://img.youtube.com/vi/cEH_ipqHbUw/sddefault.jpg)

4. **YouTube Tutorial:** [C Programming Tutorial - 44 - Simple HTTP Server](https://www.youtube.com/watch?v=2HrYIl6GpYg&pp=ygUQaHR0cCBzZXJ2ZXIgaW4gYw%3D%3D)
![YouTube Tutorial Preview](https://img.youtube.com/vi/2HrYIl6GpYg/sddefault.jpg) 
