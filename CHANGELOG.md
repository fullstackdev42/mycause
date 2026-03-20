# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.1.0] - 2024-11-23

### Added

- Web server with Echo framework and Uber FX dependency injection
- Campaign management (CRUD operations, campaign handlers, campaign service layer)
- User authentication with session management and flash messages
- Registration and login flow with session serialization
- Password recovery flow
- CSRF middleware with token injection into forms
- Database layer with migration support (up and down) and retry/backoff logic
- Structured logging with Zap logger and custom FX logger
- Configuration system with environment variable support and validation
- Health check endpoint with version reporting
- Template rendering engine with shared error handling
- Docker image build and initial deployment pipeline via GitHub Actions
- Taskfile-based development workflow
- Frontend build with Tailwind CSS
- REST API for campaigns
- DevContainer configuration for VS Code

### Changed

- Refactored session management into dedicated FX module
- Refactored campaign package structure and service layer
- Refactored template rendering to use shared data sources
- Refactored email package and removed unused mocks
- Moved flash message handling to base handler
- Moved migrations into database folder
- Simplified database connection setup with FX modules

### Fixed

- Campaign update and handler test failures
- Data access issues in campaign service
- Flash message interface inconsistencies
- Session key validation and user serialization
- API response handling for edge cases
- Environment variable defaults and production logging
