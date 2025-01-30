# GO-BLOCKCHAIN

![Block Mining Animation](https://miro.medium.com/v2/resize:fit:700/1*lU0tXETMl4nEdKxdJSaDIA.gif)

Implementing Blockchain in Golang on the Concept of Proof Of Work.

## Features

- Implemented the core blockchain structure and functionality, including the creation and validation of new blocks.
- Developed a Proof of Work algorithm that iteratively hashes new blocks until a hash meeting the difficulty criteria is found. This process ensures the computational difficulty and security of adding new blocks to the chain.
- Utilized Go's powerful concurrency features to optimize the Proof of Work process.
- Ensured the integrity of the blockchain by validating that each new block's hash is a hash of the previous block.

## Getting Started

### Prerequisites

- Go (Golang) installed on your machine.
- `curl` command-line tool for testing the API.

### Running the Application

1. Clone the repository:

    ```sh
    git clone https://github.com/yourusername/GO-BLOCKCHAIN.git
    cd GO-BLOCKCHAIN
    ```

2. Run the application:

    ```sh
    go run main.go
    ```

3. In another terminal, use `curl` to add a new block:

    ```sh
    curl -X POST -H "Content-Type: application/json" -d '{"Data": 75}' http://localhost:8092
    ```

### Explanation

- The `go run main.go` command starts the blockchain server.
- The `curl` command sends a POST request to the server to add a new block with the data `75`.
