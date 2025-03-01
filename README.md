# SocialHub
SocialHub is a simple social network platform built with microservices. Users can create posts, comment, like posts, and chat in real time.

## Features
- User registration and login
- Create, edit, and delete posts
- Comment on posts
- Like posts
- Real-time notifications
- Real-time chat between users

## Technologies
- **Backend**: Spring Boot, MongoDB, Kafka, Redis
- **Frontend**: ReactJS
- **Containerization**: Docker
- **Orchestration**: Kubernetes
- **API Gateway**: Spring Cloud Gateway

## Architecture
SocialHub uses a microservices architecture with the following main services:

1. **User Service**: 
    - Manages user registration, login, and profiles.
    - Uses JWT for secure authentication.
2. **Post Service**: 
    - Handles posts, comments, and likes.
    - Uses Redis to cache popular posts.
3. **Notification Service**: 
    - Sends real-time notifications using Kafka and WebSocket.
4. **Chat Service**: 
    - Allows users to chat in real time.
    - Uses Redis to store temporary chat messages.
5. **Gateway Service**:
   - Routes user requests to the correct service.
   - Implements rate limiting to avoid too many requests.

## Installation
### Prerequisites
- Docker
- Kubernetes
- Java 11 or higher
- Node.js and npm

### Steps
