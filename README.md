# PinjamKelas Docs

Complete documentation repository for the PinjamKelas platform, a comprehensive system designed for classroom resource sharing and management. This repository contains all technical documentation, API references, guides, and deployment instructions.

📋 Table of Contents

- Features
- Documentation Structure
- Tech Stack
- Quick Start
- Project Contents
- Contributing
- Support
- License

✨ Features

Documentation Includes

- **System Architecture**: Complete design documentation and technical specifications
- **API Reference**: Full REST API documentation with request/response examples
- **Setup Guides**: Step-by-step installation and deployment instructions
- **User Manuals**: Comprehensive guides for end-users and administrators
- **Developer Guide**: Technical documentation for developers and contributors
- **Database Schema**: Complete database design and relationships
- **Troubleshooting**: Common issues and solutions
- **Deployment Guide**: Production deployment and configuration

Repository Features

- Well-organized markdown documentation
- Code examples and best practices
- API endpoint specifications
- Database schema diagrams
- Setup and configuration guides
- Comprehensive search indexing
- Version-controlled documentation

🛠 Tech Stack

- **Format**: Markdown
- **Version Control**: Git & GitHub
- **Documentation Style**: Professional & Technical
- **Audience**: Developers, Users, Administrators
- **Search**: Full-text searchable

📁 Documentation Structure

```
docs/
├── api/                          # Backend API Documentation
│   ├── authentication.md         # Authentication & JWT
│   ├── users.md                  # User endpoints
│   ├── classrooms.md             # Classroom management
│   ├── posts.md                  # Borrowing requests
│   └── status-logs.md            # Status tracking
├── backend/                      # Backend-specific Documentation
│   ├── setup.md                  # Backend setup & prerequisites
│   ├── database-schema.md        # Database design
│   └── deployment.md             # Backend deployment
├── frontend/                     # Frontend Documentation
│   ├── setup.md                  # Frontend setup & prerequisites
│   ├── components.md             # Component structure & usage
│   ├── api-integration.md        # API integration guide
│   ├── styling.md                # UI/UX & styling guidelines
│   └── responsive-design.md      # Mobile & responsive design
├── guides/                       # General Setup Guides
│   ├── getting-started.md        # Quick start guide
│   ├── installation.md           # Installation steps
│   ├── configuration.md          # Configuration guide
│   └── deployment.md             # Production deployment
├── architecture/                 # Architecture Documentation
│   ├── system-design.md          # System overview
│   ├── authentication.md         # Auth architecture
│   └── project-structure.md      # Full system structure
├── troubleshooting/              # Troubleshooting Guides
│   └── common-issues.md          # FAQ & Solutions
└── README.md                     # This file
```

🚀 Quick Start

1. **Clone the Repository**
   ```bash
   git clone https://github.com/Rezdblz/2026-PinjamKelas-Docs.git
   cd 2026-PinjamKelas-Docs
   ```

2. **Create a Local Copy**
   ```bash
   cp -r . ./local-docs
   ```

3. **View Documentation**
   - Open files in your markdown reader
   - Or view directly on GitHub

4. **Search Documentation**
   - Use GitHub's search feature
   - Or search locally with your editor

📚 Key Documentation Sections

**For Users**
- Getting Started Guide
- User Manual - Creating & Managing Requests
- Frontend Usage Guide
- FAQ & Troubleshooting

**For Frontend Developers**
- Frontend Setup & Installation
- Component Documentation
- API Integration Guide
- Responsive Design Guidelines
- Styling & UI/UX Standards
- Building & Deployment

**For Backend Developers**
- System Architecture
- Backend API Reference
- Database Schema
- Development Setup
- Database Migrations

**For Administrators**
- Deployment Guide
- Configuration Reference
- Maintenance Procedures
- User Management

📝 Documentation Standards

All documentation follows these standards:

- Clear, concise language
- Proper markdown formatting
- Code examples where applicable
- Updated version information
- Functional links and references
- Version control through Git

💻 Frontend Tech Stack

- **Framework**: React 18 with TypeScript
- **Build Tool**: Vite
- **Styling**: Tailwind CSS
- **State Management**: React Hooks & Context API
- **HTTP Client**: Fetch API
- **Routing**: React Router
- **Form Handling**: Custom React Hooks

**Frontend Features**

- User Authentication with role-based access
- Create & manage borrowing requests
- Real-time search and filtering
- Responsive design (Mobile, Tablet, Desktop)
- Dark theme UI with Tailwind CSS
- Admin approval/rejection interface
- Detailed request modal views

**Frontend Quick Setup**

```bash
# Clone repository
git clone https://github.com/Rezdblz/2026-PinjamKelas-Frontend.git
cd 2026-PinjamKelas-Frontend/PinjamKelas

# Install dependencies
npm install

# Configure API endpoint
# Create .env file with: VITE_API_URL=http://localhost:3000/api

# Start dev server
npm run dev

# Access at http://localhost:5173
```

⚙️ Backend Tech Stack

- **Framework**: .NET 10.0 ASP.NET Core
- **ORM**: Entity Framework Core (EF Core)
- **Database**: PostgreSQL
- **Authentication**: JWT (JSON Web Tokens)
- **API Docs**: Swagger/OpenAPI
- **Language**: C#

**Backend Features**

- Secure JWT-based authentication
- RESTful API endpoints for all resources
- Role-based access control (Student/Admin)
- Automatic status logging and audit trails
- Soft delete implementation
- CORS support
- Comprehensive API documentation
- Database seeding for development

**Backend Quick Setup**

```bash
# Clone repository
git clone https://github.com/Rezdblz/2026-PinjamKelas-Backend.git
cd 2026-PinjamKelas-Backend/PinjamKelas.Api

# Restore dependencies
dotnet restore

# Configure database
# Update connection string in appsettings.json or .env

# Apply migrations
dotnet ef database update

# Start dev server
dotnet run

# Access Swagger at http://localhost:5000/swagger
```

🔑 API Quick Reference

Authentication
```
POST /api/auth/login
Authorization: Bearer <token>
```

Users
```
GET /api/users                    # List all users
POST /api/users                   # Create user
GET /api/users/{id}              # Get user details
PUT /api/users/{id}              # Update user
DELETE /api/users/{id}           # Delete user
```

Classrooms
```
GET /api/classrooms              # List classrooms
POST /api/classrooms             # Create classroom
GET /api/classrooms/{id}         # Get details
PUT /api/classrooms/{id}         # Update classroom
DELETE /api/classrooms/{id}      # Delete classroom
```

Posts (Borrowing Requests)
```
GET /api/posts                   # List posts
POST /api/posts                  # Create post
GET /api/posts/{id}             # Get post details
PUT /api/posts/{id}             # Update post
DELETE /api/posts/{id}          # Delete post
PUT /api/posts/{id}/approval    # Approve/reject
```

📊 Related Repositories

| Repository | Technology | Purpose | Status |
|-----------|-----------|---------|--------|
| [Backend API](https://github.com/Rezdblz/2026-PinjamKelas-Backend) | .NET Core, PostgreSQL | REST API for resource management | Active |
| [Frontend Web](https://github.com/Rezdblz/2026-PinjamKelas-Frontend) | React, TypeScript, Tailwind | Web application UI | Active |
| [Documentation](https://github.com/Rezdblz/2026-PinjamKelas-Docs) | Markdown | Comprehensive documentation | Active |

**Getting Started with Multiple Repos**

To set up the complete PinjamKelas system:

1. **Start the Backend**
   - Clone backend repository
   - Follow backend setup guide (see above)
   - API runs at `http://localhost:5000`
   - Swagger UI at `http://localhost:5000/swagger`

2. **Start the Frontend**
   - Clone frontend repository
   - Follow frontend setup guide (see above)
   - Update `VITE_API_URL` to point to backend
   - Frontend runs at `http://localhost:5173`

3. **Access the Application**
   - Open `http://localhost:5173` in browser
   - Create account or login with seeded credentials
   - Start managing borrowing requests

🤝 Contributing

Contributions to improve documentation are welcome!

Guidelines:

- Use clear, professional language
- Follow markdown formatting standards
- Include examples where helpful
- Update related documentation
- Add timestamps for changes
- Test all links before submitting

Steps:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request
5. Include description of changes

💬 Support & Contact

- **Issues**: Open an issue on GitHub
- **Discussions**: Use GitHub Discussions
- **Contact**: Reach out to project maintainers
- **FAQ**: Check troubleshooting guide

🗂️ Project Information

- **Owner**: Dimas Reza A (Rezdblz)
- **Status**: Active Development
- **Last Updated**: February 17, 2026
- **Version**: 1.0.0

## License

MIT License - see [LICENSE](LICENSE) for details.

---

**Copyright © 2026 Dimas Reza A** | All Rights Reserved