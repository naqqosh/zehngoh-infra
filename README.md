# Zehngoh Infrastructure

Infrastructure repository for Zehngoh local commerce platform.

## Overview

Zehngoh is a Telegram-based local commerce and delivery platform serving rural communities in Uzbekistan.

## Production Metrics

- 42 registered users
- 11 active sellers
- 160+ orders processed
- 290+ products
- 6+ months in production

## Architecture

User → Telegram Bot → Next.js Web App → NestJS API → PostgreSQL

![Architecture diagram](https://github.com/user-attachments/assets/f8c34ea7-d366-4140-b38a-c2f5d109df9c)

## Infrastructure Stack

- Docker
- Docker Compose
- GitHub Actions
- GitHub Container Registry (GHCR)
- DigitalOcean VPS
- Nginx
- SSL

## CI/CD Flow

1. Push to main branch
2. GitHub Actions builds Docker images
3. Images pushed to GHCR
4. SSH connection to production server
5. docker compose pull
6. docker compose up -d

## Services

- nginx
- ui
- api
- postgres

## Repository Purpose

Contains deployment configuration, CI/CD workflows and production infrastructure setup.
