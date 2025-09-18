# 🛡️ API Gateway - Mini E-Commerce

The **API Gateway** is the single entrypoint for clients (Web, Mobile) in the **Mini E-Commerce Shop** system.  
It exposes **REST endpoints** and proxies requests to backend microservices using **gRPC**.

---

## 🚀 Features
- REST API for clients
- JWT Authentication (via Auth Service)
- gRPC clients for internal services
- Middleware support (Auth, Logging, Metrics)
- Built with **Go + Chi + gRPC**

---

## 📂 Project Structure
api-gateway/
 ├── cmd/               # Entry point
 ├── internal/
 │   ├── config/        # Load env/config
 │   ├── server/        # HTTP server setup
 │   ├── routes/        # Route definitions
 │   ├── handlers/      # REST handlers
 │   ├── clients/       # gRPC clients
 │   ├── middleware/    # JWT, logging, metrics
 │   └── utils/         # JSON response helpers
 ├── proto/             # Protobuf definitions + generated code
 └── go.mod
