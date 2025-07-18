# ⚡ Nx Monorepo – API Gateway + Auth Service

This is an Nx-based monorepo designed using microservice architecture principles. It includes an **API Gateway** and an **Authentication Service**, each with its own **E2E tests**, built for scalable enterprise-grade backend systems.

---

## 🏗️ Tech Stack

- **Monorepo Tooling**: [Nx.dev](https://nx.dev)
- **Language**: TypeScript
- **Framework**: Express.js (Node.js)
- **API Gateway**: Custom gateway (Express)
- **Auth Service**: Token-based authentication (JWT)
- **Testing**: Cypress / Jest (E2E and Unit)

---

## 📁 Folder Structure

apps/
api-gateway/ → Entry point for routing requests
auth-service/ → Authentication microservice
api-gateway-e2e/ → End-to-end tests for API Gateway
auth-service-e2e/ → End-to-end tests for Auth Service

libs/
(optional) shared utilities or models

nx.json → Nx workspace configuration
project.json → Project definitions
workspace.json → Legacy config (if present)

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/your-repo.git
cd your-repo
npm install
npx nx serve api-gateway
npx nx serve auth-service

Or run them in parallel using:

npx nx run-many --target=serve --all

npx nx e2e api-gateway-e2e
npx nx e2e auth-service-e2e
