# KopStadium v2

> A modern, scalable table-booking and community platform for sports fans, bars and administrators.

## 🚀 Project Overview

KopStadium v2 is a full-stack web application designed to let users reserve tables to watch live matches, allow bars to publish and manage their availability, and give administrators a central dashboard to oversee the entire ecosystem. Built from the ground up with production-ready architecture, strong typing, automated testing, and CI/CD pipelines.

### Key Features

- **User Interface**  
  - Browse upcoming matches and available bars  
  - Book & manage table reservations  
  - Participate in fan forum (posts, comments, voting)  

- **Bar Owner Interface**  
  - CRUD on bar profiles and table inventory  
  - View & manage incoming reservations  
  - Publish special match-day events  

- **Admin Interface**  
  - Approve new bars and content  
  - View system metrics & reservation analytics  
  - Manage user roles and permissions  

- **Advanced Services**  
  - Real-time availability & notifications  
  - Machine-learning powered ad targeting  
  - Integration with external sports APIs (e.g. match schedules, live stats)  

---

## 📂 Repository Structure

```text
kopstadium/
├── backend/            # Node.js + TypeScript REST API
│   ├── src/
│   │   ├── controllers/
│   │   ├── services/
│   │   ├── repositories/
│   │   ├── dtos/
│   │   ├── middlewares/
│   │   └── utils/
│   ├── Dockerfile
│   ├── tsconfig.json
│   └── package.json
├── frontend/           # Next.js + React application
│   └── …
├── infra/              # Infrastructure as code & Docker Compose
│   └── docker-compose.yml
├── .env.example
├── package.json        # Monorepo workspaces
├── README.md
└── CONTRIBUTING.md
🛠 Tech Stack
Backend: Node.js, TypeScript, Express (or NestJS), Prisma ORM, PostgreSQL, Redis

Frontend: Next.js, React, TypeScript, Tailwind CSS

Infrastructure: Docker, Docker Compose, GitHub Actions, Railway / Vercel deployments

Testing: Jest, Supertest (backend), React Testing Library (frontend)

Documentation: OpenAPI (Swagger), Redoc

⚙️ Getting Started
Prerequisites
Node.js v18+

Docker & Docker Compose

Clone & Install
git clone https://github.com/your-org/kopstadium.git
cd kopstadium
npm ci
Environment Variables
Copy and update .env.example at the root:

bash
Copiar
Editar
cp .env.example .env
# Edit .env with your own values for:
# PORT, DATABASE_URL, REDIS_URL, JWT_SECRET, etc.
Local Development
Bring up services

npm run docker:up
Backend
npm run dev:backend

Frontend
npm run dev:frontend
Access:

Backend API → http://localhost:3000

Frontend App → http://localhost:3001

🧪 Testing
Lint & Format

npm run lint
npm run format
Unit & Integration Tests

npm test
Health-check

curl http://localhost:3000/health
🚢 CI/CD
GitHub Actions pipeline runs on push/PR:

Checkout & cache dependencies

Lint & build

Run tests & health-check

Publish Docker image & deploy to staging/production

🤝 Contributing
Please see CONTRIBUTING.md for:

Branch & commit conventions (Conventional Commits)

Pull request guidelines

Code review checklist

📄 License 2025 Neil Muñoz Lago aka Neiland85
This project is licensed under Apache 2.0 License. See LICENSE for details.
                           Version 2.0, January 2004
                        http://www.apache.org/licenses/
