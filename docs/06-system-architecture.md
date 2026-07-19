# System Architecture

## Version History

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | July 2026 | Saleha Pathan | Initial architecture document |

---

# 1. Purpose

This document defines the overall software architecture of the 4 Star Boutiqueen e-commerce platform. It describes the application's components, technology stack, communication flow, deployment strategy, and architectural decisions.

---

# 2. Architecture Style

The application follows a **3-Tier Architecture**.

Presentation Layer
- React + Vite
- Tailwind CSS

Business Layer
- Spring Boot
- Spring Security
- REST API

Data Layer
- PostgreSQL
- Spring Data JPA (Hibernate)

---

# 3. High-Level Architecture

Customer
↓
React Frontend
↓ REST API
Spring Boot Backend
↓
PostgreSQL Database

External Services

Cloudinary (Product Images)

GitHub Actions (CI/CD)

AWS EC2 (Hosting)

AWS RDS (Database)

---

# 4. Technology Stack

| Layer | Technology | Reason |
|--------|------------|--------|
| Frontend | React + Vite | Fast, modern frontend framework |
| Styling | Tailwind CSS | Utility-first responsive design |
| Backend | Spring Boot | Enterprise Java framework |
| Language | Java 21 | Modern LTS version |
| Build Tool | Maven | Dependency management |
| Database | PostgreSQL | Reliable relational database |
| ORM | Spring Data JPA | Simplifies database interaction |
| Authentication | Spring Security + JWT | Secure authentication |
| Image Storage | Cloudinary | Cloud image management |
| Version Control | Git & GitHub | Source control |
| Project Management | Jira | Agile project management |
| CI/CD | GitHub Actions | Automated build & deployment |
| Cloud Hosting | AWS EC2 | Production server |
| Database Hosting | AWS RDS | Managed PostgreSQL database |
| Reverse Proxy | Nginx | Routing and SSL |
| SSL | Let's Encrypt | HTTPS security |

---

# 5. Major Components

## Frontend

Responsibilities

- Display products
- Customer authentication
- Shopping cart
- Wishlist
- Checkout
- Responsive UI

---

## Backend

Responsibilities

- Business logic
- Authentication
- Order processing
- Payment integration
- Inventory management
- Admin operations

---

## Database

Responsibilities

- Store customers
- Store products
- Store orders
- Store categories
- Store reviews
- Store charity records

---

# 6. Design Principles

- Layered Architecture
- Separation of Concerns
- RESTful API Design
- Responsive Design
- Security by Design
- Scalability
- Maintainability

---

# 7. Non-Functional Requirements

- Responsive on desktop, tablet, and mobile
- Secure authentication
- Fast page loading
- High availability
- Scalable architecture
- Easy maintenance

---

# 8. Future Enhancements

- AI Outfit Try-On
- AI Personal Stylist
- Product Recommendation Engine
- Mobile Application
- Multi-language Support
- Multi-currency Support