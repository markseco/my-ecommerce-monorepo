## E-Commerce Microservices Monorepo

Currently working on the project, this is what is expected to come out of the project.

## Overview

This monorepo houses the source code for an e-commerce backend built using microservices architecture. The project consists of three main services – User API (NodeJS), Product API (Go), and Order Service (Java) – orchestrated through Kubernetes. Each service is encapsulated within its respective package, promoting modularity and ease of development.

## Features

- **User API (NodeJS):**
  - Manages user-related functionalities.
  - Utilizes S3 for user photo storage.
  - Stores user information in MongoDB.

- **Product API (Go):**
  - Handles product-related functionalities.
  - Stores product data in PostgreSQL.
  - Uses a message queue for asynchronous tasks.

- **Order Service (Java):**
  - Manages the order lifecycle.
  - Communicates with the Product API for inventory management.
  - Uses its own database for order information.

## Tech Stack

- User API: NodeJS, MongoDB, S3
- Product API: Go, PostgreSQL, Message Queue
- Order Service: Java, PostgreSQL
- Orchestration: Kubernetes
- Shared Code: Centralized in the 'shared' package