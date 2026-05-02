# 🍛 Oru Idli

Location-aware food discovery platform built for discovering the best local food spots through short-form content.

## Overview

Oru Idli combines geo-based food discovery with short-form social content. Users can upload food reels and photos tied to real-world food spots, discover trending places nearby, rate dishes, and navigate directly to restaurants and street-food locations.

The platform is designed as a scalable MVP using:

* **Flutter** for the mobile application
* **Django + DRF** for the backend API
* **PostGIS** for geo-location queries
* **Redis + Celery** for async processing and caching
* **AWS S3 + CloudFront** for media storage and delivery

The feed ranking system uses a composite scoring engine based on:

* likes
* ratings
* user credibility
* recency decay

This architecture is documented in the internal system design brief. fileciteturn0file0

---

## Core Features

* 📍 Location-based food discovery feed
* 🎥 30-second food reels
* ⭐ Ratings and reviews
* ❤️ Likes, saves, and comments
* 🗺 Food spot navigation integration
* 🔍 Smart category-based exploration
* ⚡ Real-time ranking engine
* ☁ Scalable media pipeline

---

## Architecture

```text
Flutter App
    ↓
Django REST API
    ↓
PostgreSQL + PostGIS
    ↓
Redis Cache + Celery Workers
    ↓
S3 + CDN Media Delivery
```

---

## Tech Stack

| Layer         | Technology           |
| ------------- | -------------------- |
| Mobile App    | Flutter              |
| Backend       | Django + DRF         |
| Database      | PostgreSQL + PostGIS |
| Cache         | Redis                |
| Async Jobs    | Celery               |
| Search        | Meilisearch          |
| Media Storage | AWS S3               |
| CDN           | CloudFront           |
| Deployment    | Docker               |

---

## Repositories

| Repository         | Description                           |
| ------------------ | ------------------------------------- |
| `oru-idli-app`     | Flutter mobile application            |
| `oru-idli-backend` | Django backend API                    |
| `oru-idli-infra`   | Infrastructure and deployment configs |

---

## Vision

Build the best hyperlocal food discovery platform focused on authentic community-driven recommendations.

---

## Organization Setup

To display this on the GitHub Organization overview page:

1. Create a repository named:

```text
.github
```

2. Inside that repo create:

```text
profile/README.md
```

3. Paste this content into `README.md`

GitHub automatically shows it on the organization overview page.
