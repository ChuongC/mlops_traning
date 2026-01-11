# MLOps Training

**Hands-on training for MLOps infrastructure, deployment, and CI/CD**

## Quick Start

### Option 1: View Documentation as Website (Recommended)

The documentation is built with **VitePress** and can be viewed as an interactive website:

```bash
# 1. Install dependencies
npm install

# 2. Start the documentation server
npm run docs:dev

# 3. Open in browser
# Documentation will be available at http://localhost:5173
```

**Features**:
- 📖 Clean, readable interface
- 🔍 Built-in search functionality
- 📱 Mobile-responsive design
- 🎨 Syntax highlighting for code blocks
- 🔄 Hot-reload during development

### Option 2: Read Markdown Directly

Browse the [Study Guide](./docs/) in the `docs/` folder directly:

```
Start here:  docs/README.md  →  Complete study guide
Then:        module-01/      →  Hands-on labs
```

## Course Overview

| Module | Topic | Description | Technologies |
|--------|-------|-------------|--------------|
| 1 | Infrastructure & Prerequisites | Docker, AWS, Terraform fundamentals | Docker, AWS, Terraform, LocalStack |
| 2 | Model Deployment | Batch, API, streaming deployments | FastAPI, Docker, AWS Lambda |
| 3 | Testing & CI/CD | Testing strategies and CI/CD pipelines | GitHub Actions, pytest |

## Repository Structure

```
mlops_training/
├── docs/                          # 📖 CONCEPTUAL LEARNING
│   ├── README.md                  #   Study guide and navigation
│   ├── module-01/                 #   Module 1 theory and guides
│   │   ├── docker/                #   - Docker concepts
│   │   ├── terraform/             #   - Terraform IaC guide
│   │   └── aws/                   #   - AWS CLF-C02 exam prep
│   ├── module-02/                 #   Module 2 theory
│   └── module-03/                 #   Module 3 theory
│
├── module-01/                     # 🛠️ LAB & PRACTICE CODE
│   ├── docker/basics/             #   Docker containers and compose
│   ├── terraform/basics/          #   Terraform configurations
│   └── aws/localstack/            #   LocalStack for AWS practice
│
├── module-02/                     #   Model deployment labs
│   └── batch-api/fastapi/         #   FastAPI deployment
│
├── module-03/                     #   Testing and CI/CD labs
│   └── testing/                   #   Testing frameworks
│
└── assets/                        # Images and diagrams
```

## How to Use This Training

### For Each Topic

1. **Read the theory** in `docs/module-X/`
2. **Practice with labs** in `module-X/`
3. **Experiment** with configurations
4. **Build your own** variations

### Example: Learning Docker

```bash
# 1. Read the conceptual guide
cat docs/module-01/docker/basics.md

# 2. Navigate to the lab
cd module-01/docker/basics

# 3. Run the exercises
docker compose up -d

# 4. Experiment and learn
docker compose logs -f
```

### Example: Learning AWS with LocalStack

```bash
# 1. Read AWS service guide
cat docs/module-01/aws/storage-services.md

# 2. Start LocalStack
cd module-01/aws/localstack
cp .env.example .env
docker compose up -d

# 3. Practice S3 operations
aws --endpoint-url=http://localhost:4566 s3 mb s3://my-bucket
```

## Viewing Documentation with VitePress

This project uses **VitePress** to provide a beautiful, searchable documentation website.

### Installation

```bash
# Install Node.js dependencies
npm install
```

**Requirements**:
- Node.js 18.x or higher
- npm 9.x or higher

### Development Server

Start the local development server with hot-reload:

```bash
npm run docs:dev
```

Open your browser to: **http://localhost:5173**

The development server supports:
- 🔄 **Hot reload**: Changes to markdown files are instantly reflected
- 🔍 **Full search**: Search across all documentation
- 📱 **Responsive**: Works on desktop, tablet, and mobile

### Build for Production

Create a static site ready for deployment:

```bash
# Build the static site
npm run docs:build

# Preview the built site
npm run docs:preview
```

The built site will be in `docs/.vitepress/dist/` and can be deployed to:
- GitHub Pages
- Netlify
- Vercel
- Any static hosting service

### VitePress Commands

| Command | Description |
|---------|-------------|
| `npm install` | Install VitePress dependencies |
| `npm run docs:dev` | Start development server at http://localhost:5173 |
| `npm run docs:build` | Build static site for production |
| `npm run docs:preview` | Preview the production build locally |

### Customization

VitePress configuration is in `docs/.vitepress/config.ts`:
- Navigation menu
- Sidebar structure
- Theme settings
- Search configuration

## Module Guides

| Module | Study Guide | Lab Location |
|--------|-------------|--------------|
| **Module 1** | [Infrastructure Guide](./docs/module-01/) | [`module-01/`](./module-01/) |
| **Module 2** | Coming soon | [`module-02/`](./module-02/) |
| **Module 3** | Coming soon | [`module-03/`](./module-03/) |

## Prerequisites

- **Node.js** 18.x or higher (for VitePress documentation viewer)
- **npm** 9.x or higher
- Basic Python knowledge
- Machine learning concepts
- Command-line interface familiarity
- Docker Desktop installed

## Study Path

1. **[Start with the Study Guide](./docs/)** - Complete overview
2. **Module 1: Infrastructure** - Docker, Terraform, AWS
3. **Module 2: Model Deployment** - Batch and API patterns
4. **Module 3: Testing & CI/CD** - Automation pipelines

## Contributing

This is a training repository. See [CONTRIBUTING.md](./CONTRIBUTING.md)

---

## Quick Reference

```bash
# View documentation as website
npm install
npm run docs:dev
# Open http://localhost:5173

# Build for deployment
npm run docs:build
```

**Start Learning:**
- 🌐 **View as Website**: `npm run docs:dev` then open http://localhost:5173
- 📖 **Read as Markdown**: [docs/README.md](./docs/) ← Complete study guide
