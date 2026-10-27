**English** | [Ελληνικά](README.el.md)

# PulseGuard
![CI](https://github.com/aggelosklaudianos-gif/pulseguard/actions/workflows/ci.yml/badge.svg)

Cloud-native platform for remote monitoring of patients with hypertension.
Patients record blood pressure readings at home; the system evaluates them
against clinical rules and alerts the treating physician.

> Learning project. All data is synthetic. Not a medical device.

## Tech stack

Java 25 · Spring Boot 4.1 · PostgreSQL + TimescaleDB · Docker

## Run locally

Requirements: JDK 25, Docker Desktop

    docker compose up -d
    cd core-service
    ./mvnw spring-boot:run

Health check: http://localhost:8080/actuator/health

## Status

- [x] Phase 0: Project foundations
- [ ] Phase 1: Core (patients, measurements, statistics)
- [ ] Phase 2: Security
- [ ] Phase 3: FHIR interoperability
- [ ] Phase 4: Real-time ingestion and alerts
- [ ] Phase 5: Cloud deployment