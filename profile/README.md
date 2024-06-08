# Skitters

Skitters is a task management software developed by CraftNotion, designed to simplify the tracking of clients, projects, and tasks.

## Technologies Used

### Frontend
- **Framework**: Next.js
- **Styling**: SASS

### Backend
- **Microservices Framework**: NestJS
- **Database**: PostgreSQL
- **Search Engine**: Elasticsearch

## Microservices

Skitters consists of the following microservices, each running in microservice mode and exposing ports for internal communication, WebSocket, and HTTPS.

| Service         | Description                                     | Internal Port | WebSocket Port | HTTPS Port |
|-----------------|-------------------------------------------------|---------------|----------------|------------|
| Authentication  | Manages user authentication and authorization   | 3001          | 5001           | 4001       |
| Project         | Handles project management and tracking         | 3002          | 5002           | 4002       |
| Communication   | Manages client communication and notifications  | 3003          | 5003           | 4003       |
| Elastic         | Provides search functionality using Elasticsearch| 3004          | 5004           | 4004       |

## Getting Started

### Prerequisites
- Node.js
- PostgreSQL
- Elasticsearch

### Installation

1. Clone the repositories for each microservice:
   ```bash
   git clone https://github.com/Craftnotion-Skitters/authentication-service.git
   git clone https://github.com/Craftnotion-Skitters/project-service.git
   git clone https://github.com/Craftnotion-Skitters/communication-service.git
   git clone https://github.com/Craftnotion-Skitters/elastic-service.git
   ```

2. Navigate to each microservice directory and install dependencies:
   ```bash
   cd authentication-service
   npm install
   cd ../project-service
   npm install
   cd ../communication-service
   npm install
   cd ../elastic-service
   npm install
   ```

### Running the Services

1. Start PostgreSQL and Elasticsearch.

2. Run each service:
   ```bash
   # In each service directory
   npm run start
   ```

3. Start the frontend application:
   ```bash
   cd frontend
   npm install
   npm run dev
   ```

### Environment Variables

Ensure each service has the required environment variables set. Refer to `.env.example` files in each repository for necessary configurations.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Contact

For any questions or support, please contact us at support@craftnotion.com.

---

And here's the short description for GitHub:

---

**Skitters** is a task management software by CraftNotion, designed to simplify the tracking of clients, projects, and tasks. Built with Next.js and SASS on the frontend, and NestJS, PostgreSQL, and Elasticsearch on the backend, it leverages a microservices architecture to efficiently manage authentication, projects, communication, and search functionality.
