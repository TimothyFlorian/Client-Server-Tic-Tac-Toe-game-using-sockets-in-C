# Tic-Tac-Toe Online

Welcome to Tic-Tac-Toe Online! This project enables multiple players to enjoy the classic game of Tic-Tac-Toe over a network connection. Players can connect to a central server and compete against each other in real-time.

## Getting Started

To get started with Tic-Tac-Toe Online, follow these instructions:

### Prerequisites

- You need a C compiler installed on your system. If you don't have one already, you can install `gcc`.

### Server Setup

1. Compile the server code:
    ```bash
    gcc -pthread server.c -o server
    ```

2. Run the server, specifying the desired port number (e.g., 5552):
    ```bash
    ./server 5552
    ```

### Client Setup

1. Compile the client code:
    ```bash
    gcc client.c -o client
    ```

2. Connect the first client to the server by providing the server's IP address (e.g., 172.22.105.145) and the port number used for the server (e.g., 5552):
    ```bash
    ./client 172.22.105.145 5552
    ```

3. Connect the second client similarly, providing the same server IP address and port number.

### Gameplay

- Once both clients are connected, they can take turns making moves in the Tic-Tac-Toe game.
- Follow the on-screen prompts to enter your moves.
- The game ends when one player wins, there's a draw, or a player disconnects.

## Contributing

Contributions to Tic-Tac-Toe Online are welcome! If you have any ideas for improvements or new features, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
