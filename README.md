# Tlhophego Naphtaly Mathye
**Solutions Developer · Java Backend · React Native · React Web**  
*Building robust backends and seamless mobile experiences*

📍 Pretoria, South Africa &nbsp;|&nbsp; [LinkedIn](https://www.linkedin.com/in/tnmathye) &nbsp;|&nbsp; [tlhophegom@gmail.com](mailto:tlhophegom@gmail.com) &nbsp;|&nbsp; [+27 69 729 3172](tel:+27697293172) &nbsp;|&nbsp; [WhatsApp](https://wa.me/27697293172)

---

## About Me

I'm a **Solutions Developer** with **3 years of experience** based in Pretoria, South Africa, originally from Polokwane, Moletjie. I specialise in low-code/no-code development as part of my current role, and I am deeply passionate about crafting high-quality mobile applications and web solutions.

This repository is dedicated to my personal growth and portfolio work in:
- **Java Backend Development** with the Spring Framework
- **Mobile Development** with React Native
- **Web Development** with React

I believe in writing clean, maintainable code and continuously improving through hands-on projects.

---

## Tech Stack

**Languages**  
Java, JavaScript, TypeScript

**Frameworks & Libraries**  
Spring, Spring Boot, React, React Native

**Databases**  
PostgreSQL, MySQL, MongoDB

**Tools & Platforms**  
Git, GitHub, VS Code, IntelliJ IDEA

---

## Projects Overview

> All repositories listed below are **private**.

| Project | Type | Status | Description |
|---|---|---|---|
| [🛒 E-Commerce Modular Monolith](#-e-commerce-modular-monolith) | Java · Spring Boot | ![Status](https://img.shields.io/badge/status-in%20progress-blue) | Production-grade e-commerce backend with modular architecture, JWT auth, and role-based access control |
| [🛍️ ShopZA](#️-shopza) | React Native · Expo | ![Status](https://img.shields.io/badge/status-in%20progress-blue) | Mobile e-commerce frontend with JWT auth, onboarding flow, and home feed — client for the modular monolith |
| [🔐 Spring Boot JWT Authentication](#-spring-boot-jwt-authentication) | Java · Spring Boot | ![Status](https://img.shields.io/badge/status-complete-brightgreen) | Foundational RESTful API with JWT-based authentication, user registration, and protected routes |
| [🌱 MasterSpring APIs](#-masterspring-apis) | Java · Spring Boot | ![Status](https://img.shields.io/badge/status-on%20pause-yellow) | Progressive Spring Boot learning project — paused while the e-commerce and ShopZA projects are active |

---

### 🛒 E-Commerce Modular Monolith
> *Private Repository* &nbsp; ![Status](https://img.shields.io/badge/status-in%20progress-blue)

A production-grade e-commerce backend built as a **Modular Monolith** using Spring Boot 3.5 and Java 21. The architecture enforces strict module boundaries — each module exposes only a published Java interface, and all cross-module access rules are verified at compile time via ArchUnit.

**Tech:** Java 21 · Spring Boot 3.5 · Spring Security · JWT (JJWT) · MapStruct · Flyway · PostgreSQL · H2 · ArchUnit · Swagger UI

**Highlights:**
- Two-token auth model — short-lived JWT access tokens with rotating opaque refresh tokens stored in the database
- Role-based access control: `ROLE_USER`, `ROLE_ADMIN`, `ROLE_STORE_OWNER`
- Modular Monolith with ArchUnit-enforced module boundaries — violations fail the build
- Full user CRUD with soft-delete, optimistic locking, and Flyway-managed migrations
- Swagger UI and H2 console available in dev; PostgreSQL in production

**Planned Modules:** `product`, `order`, `payment`, `notification`

**Mobile client:** [ShopZA — React Native Frontend](#️-shopza)

---

### 🛍️ ShopZA
> *Private Repository* &nbsp; ![Status](https://img.shields.io/badge/status-in%20progress-blue)

A React Native (Expo) mobile e-commerce application built for the South African market. ShopZA is the mobile frontend client for the E-Commerce Modular Monolith backend, implementing a full JWT authentication flow with access token + refresh token lifecycle management.

**Tech:** React Native · Expo · TypeScript · NativeWind (Tailwind CSS) · Expo Router · Expo SecureStore · AsyncStorage

**Highlights:**
- 7-slide onboarding shown only on first launch, skipped on return visits
- Silent JWT token refresh via `authFetch` — transparent to the user
- `RouteGuard` centralises all redirect logic; screens are auth-agnostic
- Home feed with store cards and horizontal product rows (mock data, API-ready)
- Reusable atomic UI component library: buttons, inputs, banners, state screens
- South African design tokens in a central `theme.ts`

**Backend:** [E-Commerce Modular Monolith](#-e-commerce-modular-monolith)

---

### 🔐 Spring Boot JWT Authentication
> *Private Repository* &nbsp; ![Status](https://img.shields.io/badge/status-complete-brightgreen)

A RESTful API implementing JWT-based authentication and authorization using Spring Boot and Spring Security. This project demonstrates secure user registration, login, and protected route access using JSON Web Tokens — the foundational auth concepts that evolved into the more advanced implementation in the E-Commerce Modular Monolith.

**Tech:** Java · Spring Boot · Spring Security · JWT · PostgreSQL · MySQL

**Highlights:**
- Secure signup and signin endpoints with JWT token issuance
- Role-based access control with protected and public routes
- Environment variable configuration to keep secrets out of source control
- Clean layered architecture: controller → DTO → entity → repository → security

---

### 🌱 MasterSpring APIs
> *Private Repository* &nbsp; ![Status](https://img.shields.io/badge/status-on%20pause-yellow)

A progressive Spring Boot learning project built from the ground up to grow from foundational concepts to production-ready mastery. Currently paused while the E-Commerce Modular Monolith and ShopZA projects are active — the concepts explored here feed directly into both of those projects.

**Tech:** Java 17+ · Spring Boot 3.x · Spring Data JPA · Jakarta Bean Validation · Lombok · Maven · PostgreSQL · H2

**Highlights:**
- Custom `@PasswordMatches` constraint — class-level validator comparing `password` and `confirmPassword` fields
- Custom `@ValidSAId` constraint — validates a 13-digit South African ID number including Luhn algorithm checksum
- `BaseModel` abstract entity with auto-managed `createdAt` / `updatedAt` via JPA lifecycle hooks
- Domain modelling: `User`, `Profile`, `Role` with full validation and DTO layer

**Phase 1 (Foundation) complete.** Phases 2–6 cover persistence, REST API, security, advanced features, and production readiness.

---

## Current Focus

- Deepening expertise in **Spring Boot** microservices and RESTful API design
- Building **React Native** mobile apps from concept to deployment
- Expanding **React** web development skills with modern patterns and best practices
- Exploring advanced database design with **PostgreSQL** and **MongoDB**

---

## Get In Touch

I'm always open to connecting with fellow developers, collaborating on interesting projects, or simply exchanging ideas.

- **LinkedIn:** [linkedin.com/in/tnmathye](https://www.linkedin.com/in/tnmathye)
- **Primary Email:** [tlhophegom@gmail.com](mailto:tlhophegom@gmail.com)
- **Secondary Email:** [tlhophegomathye@gmail.com](mailto:tlhophegomathye@gmail.com)
- **Phone / WhatsApp:** [+27 69 729 3172](https://wa.me/27697293172)

---

*"Great software is built one commit at a time."*
