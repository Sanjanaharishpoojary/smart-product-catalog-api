# Environment Setup Guide

## 1. Project Overview

**Project:** Smart Product Catalog API

**Purpose:** Build a REST API using Java and Spring Boot, with MySQL for persistent storage and Redis for caching.

**Development environment:** Windows with local Docker containers.

**Project location:**
`D:\MyDevelopment\Projects\ProductCatalog`

**GitHub repository:**
https://github.com/Sanjanaharishpoojary/smart-product-catalog-api

## 2. System Environment

| Component | Details |
|---|---|
| Operating System | Windows |
| Processor architecture | AMD64 |
| RAM | 8 GB |
| Project storage | D drive |
| Docker storage | D drive |
| Development approach | Local development |

## 3. Java Development Kit (JDK)

### Installed versions

- Java 21.0.13 LTS (Eclipse Temurin)
- Java 17.0.12 (existing installation)

### Primary Java version

Java 21.0.13 is configured as the primary development version.

**Installation path:**

`C:\Users\sanja\AppData\Local\Programs\Eclipse Adoptium\jdk-21.0.13.9-hotspot`

### Environment variables

`JAVA_HOME`:

`C:\Users\sanja\AppData\Local\Programs\Eclipse Adoptium\jdk-21.0.13.9-hotspot`

The Java `bin` directory is included in the system PATH.

### Verification commands

```cmd
java -version
javac -version
echo %JAVA_HOME%
```

**Verified output:**

- Java: 21.0.13
- Java compiler: 21.0.13
- JAVA_HOME points to JDK 21.

Java 21 will be used for the Spring Boot application.

## 4. Visual Studio Code

**IDE:** Visual Studio Code

**Installation path:**

`C:\Users\sanja\AppData\Local\Programs\Microsoft VS Code`

### Extensions

- Extension Pack for Java

GitHub account authentication is also configured in VS Code.

## 5. Git Configuration

**Git version:** 2.56.1.windows.1

### Verification

```bash
git --version
```

### Git identity

```bash
git config --global user.name
git config --global user.email
```

Configured identity:

- Username: `sanjanahpoojary`
- Email: `sanjanaharishpoojary@gmail.com`

### Repository initialization

The project directory was initialized as a Git repository.

```bash
git init
git branch -m main
```

Current branch: `main`

### Remote repository

```bash
git remote add origin https://github.com/Sanjanaharishpoojary/smart-product-catalog-api.git
```

Verify the remote:

```bash
git remote -v
```

### Initial commit

```bash
git add .gitignore
git commit -m "chore: add initial gitignore"
git push -u origin main
```

**Initial commit ID:** `159dee9`

The first commit was successfully pushed to GitHub.

## 6. GitHub

**Repository:** smart-product-catalog-api

**Visibility:** Public

**Repository URL:**

https://github.com/Sanjanaharishpoojary/smart-product-catalog-api

The local Git repository is connected to GitHub through the HTTPS remote named `origin`.

Authentication through Git Credential Manager is working.

## 7. Docker Desktop

**Docker Desktop version:** 4.99.0

**Docker Engine version:** 29.9.3

**Docker API version:** 1.56

**Platform:** Linux AMD64

**Docker context:** desktop-linux

### Installation configuration

- Per-user installation.
- WSL 2 backend selected.
- Docker Engine running successfully.
- Virtualization enabled in BIOS/system configuration.

### Docker storage location

Docker's disk image location was moved from the default C drive location to:

`D:\MyDevelopment\DockerData`

Docker manages its own disk image files inside this location.

### Verification commands

```bash
docker --version
docker version
```

Both Docker Client and Server were verified.

### First container test

```bash
docker run hello-world
```

**Result:** Successful.

Docker downloaded the `hello-world` image, created a container, executed it and displayed:

`Hello from Docker!`

This confirmed that Docker Desktop and the Docker Engine are working.

## 8. WSL 2

Windows Subsystem for Linux (WSL 2) is configured for Docker Desktop.

### Verification commands

```cmd
wsl --status
wsl --list --verbose
```

- Default WSL version: 2
- Docker Desktop uses WSL 2.
- A separate Ubuntu distribution is not required for this setup.

## 9. Project Directory Structure

The main development folders are:

```text
D:\MyDevelopment\
│
├── Projects\
│   ├── ProductCatalog\
│   └── JavaPractice\
│
├── Tools\
│
└── DockerData\
```

## 10. Current Project Setup Status

### Completed

- Java 21 installed and configured.
- Visual Studio Code installed.
- Java extension pack installed.
- Git installed and configured.
- Project folder created.
- Git repository initialized.
- Main branch configured.
- `.gitignore` created.
- First Git commit created.
- GitHub repository created.
- Local repository connected to GitHub.
- First commit pushed successfully.
- Docker Desktop installed.
- Docker storage moved to D drive.
- WSL 2 configured.
- Docker Engine verified.
- `hello-world` container executed successfully.

### Pending

- Spring Boot project generation.
- Maven Wrapper verification.
- MySQL container setup.
- Redis container setup.
- Docker Compose configuration.
- Postman installation.
- Database connection.
- Redis integration.
- REST API implementation.
- Unit and integration testing.

## 11. Important Development Decisions

1. Use Java 21 as the primary Java version.
2. Use Spring Boot for backend development.
3. Use MySQL as the primary database.
4. Use Redis as the caching layer.
5. Use Docker Compose to manage local infrastructure.
6. Keep project files and Docker data on the D drive.
7. Use Git for version control.
8. Use GitHub for source-code hosting and collaboration.
9. Keep passwords and sensitive configuration out of GitHub.
10. Maintain technical documentation throughout development.

---

**Document status:** Initial environment setup completed.

**Last updated:** 15 November 2026