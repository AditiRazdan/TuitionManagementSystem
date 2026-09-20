# Tuition Management System

A school-based tutoring management system designed to simplify the process of organizing and matching students with peer tutors.

This project was originally developed for use within a school **Honor Society tutoring program**, where students seeking academic support are connected with available student tutors. Traditional methods often rely on spreadsheets, forms, emails, and manual matching, which can become tedious and difficult to manage as the program grows.

The Tuition Management System provides a centralized platform for storing tutoring information and making the coordination process more efficient.

Although the system was created for a specific school use case, the code is publicly available so that other schools, Honor Societies, and student organizations can replicate, modify, or expand it for their own peer-tutoring programs.

## Purpose

School tutoring programs often require coordinators to keep track of tutoring requests, available tutors, student information, and matches across several different platforms.

Managing this information manually can be time-consuming and makes it harder to keep records organized.

This project aims to simplify that workflow by bringing tutoring information into one centralized system.

## Features

- **Tutor and student management** — stores information about students participating in the tutoring program.
- **Tutoring request management** — keeps student requests for academic support organized.
- **Tutor matching** — supports the process of connecting students with appropriate tutors.
- **User authentication** — uses ASP.NET Core Identity for secure user accounts and login.
- **Database storage** — stores tutoring and user information using SQL Server.
- **Administrative management** — allows tutoring coordinators to manage program information.
- **Persistent records** — uses Entity Framework Core to create, retrieve, update, and maintain stored data.
- **Browser-based interface** — allows users to interact with the system through a web application.
- **API documentation** — includes Swagger/Swashbuckle support.
- **Automated builds** — includes Azure Pipelines configuration for building and testing the project.

## Example Use Case

An Honor Society may have students volunteering as tutors across different subjects while other students submit requests for academic support.

Without a centralized system, coordinators may need to manually compare tutor lists and tutoring requests, contact students individually, and maintain multiple spreadsheets.

This project provides a foundation for managing these interactions in one place, reducing the administrative work involved in running a peer-tutoring program.

## Open Source / Replication

This repository is public because the problem it addresses is not unique to one school.

Other schools and student organizations can use this project as a starting point for their own Honor Society tutoring programs, peer tutoring programs, academic support organizations, or student-led tutoring initiatives.

The system can be modified depending on the needs and structure of each organization.

## Tech Stack

| Technology | Purpose |
| --- | --- |
| C# | Primary programming language |
| .NET 6 | Application framework |
| ASP.NET Core | Web application framework |
| Razor Pages | User interface |
| Entity Framework Core | Database access |
| SQL Server | Relational database |
| ASP.NET Core Identity | Authentication |
| AutoMapper | Object mapping |
| Swagger / Swashbuckle | API documentation |
| Azure Pipelines | Build and CI configuration |

## Project Structure

```text
TuitionManagementSystem-main/
│
├── Application/
├── DatabaseScripts/
├── Web/
├── TuitionManagementSystem.sln
├── azure-pipelines.yml
└── README.md
```

## Getting Started

### Prerequisites

Before running the project, make sure you have:

- Visual Studio 2022 or another IDE with .NET support
- .NET 6 SDK
- SQL Server
- SQL Server Management Studio or another SQL database management tool

### Clone the Repository

```bash
git clone https://github.com/AditiRazdan/TuitionManagementSystem-main.git
cd TuitionManagementSystem-main
```

Restore the required packages:

```bash
dotnet restore
```

## Database Setup

1. Open the scripts located in the `DatabaseScripts` directory.
2. Run the necessary scripts using SQL Server Management Studio.
3. Configure the application's SQL Server connection string.
4. Ensure SQL Server is running before launching the application.

Database credentials should be stored locally and should not be committed publicly to GitHub.

## Running the Application

Open `TuitionManagementSystem.sln` in Visual Studio and run the project.

Alternatively, use:

```bash
dotnet build
dotnet run --project Web
```

The local development URL will appear in the terminal once the application starts.

## Why This Project Exists

The goal of this project is to reduce the administrative work involved in school peer-tutoring programs.

Rather than relying on several forms, spreadsheets, and emails, coordinators can use one system to organize tutoring information and help connect students with academic support.

By making the project public, other schools can use the code as a starting point instead of having to build a similar system completely from scratch.

## Potential Future Improvements

- Automatic tutor matching based on subject and availability
- Tutoring session scheduling and notifications
- Service-hour tracking and basic program analytics
