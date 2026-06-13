# Changelog

All notable changes to this project will be documented in this file.

## [1.0.0] - 2026-04-27

### Added

- Initial release of HuggingClip
- Paperclip AI agent orchestration platform deployment on Hugging Face Spaces
- Automatic database persistence via Hugging Face Dataset backup/restore
- Health monitoring dashboard with real-time status
- PostgreSQL backup and restore functionality
- Health check endpoint for uptime monitoring
- Reverse proxy for Paperclip API and UI
- Environment variable configuration system
- Cloudflare proxy integration for network-restricted API providers
- Docker and Docker Compose support for local development
- Graceful shutdown with data synchronization
- UptimeRobot integration for preventing Space sleep
- Comprehensive documentation and guides
- MIT License

### Features

- **One-click Deploy**: Easy deployment to Hugging Face Spaces
- **Data Persistence**: Automatic backup and restore of database
- **Health Monitoring**: Dashboard showing service status and metrics
- **Flexible Configuration**: Environment variable-based configuration
- **Network Bypass**: Optional Cloudflare proxy for blocked domains
- **Local Development**: Docker Compose setup for testing
- **Extensible**: Based on Paperclip's plugin architecture

### Documentation

- README.md with deployment and usage guides
- .env.example with comprehensive configuration reference
- SECURITY.md with security best practices
- CONTRIBUTING.md with contribution guidelines
- CODE_OF_CONDUCT.md with community guidelines

## [Unreleased]

### Added

- Added `opencode-ai` CLI to agent install list (Dockerfile)
- Added OpenCode wrapper script for NODE_OPTIONS compatibility
- Added `@latest` tags to all npm-installed agent CLIs for deterministic versions
- Added `--frozen-lockfile` flag to pnpm install for reproducible builds

### Changed

- Optimized Dockerfile builder stage: removed redundant `ls -la` layer
- Multi-stage Dockerfile structure maintained for optimal image size

### Planned

- Multi-Space federation support
- Backup versioning and rotation policies
- Advanced monitoring integrations (Prometheus, Grafana)
- One-click restore from specific backup snapshots
- CLI tool for local backup management
- Multi-database support (external PostgreSQL)
- Kubernetes deployment manifests
- Better Auth integration improvements
- Agent plugin marketplace
