
# Project Architecture

## Overview

The project contains two web application containers
and one Portainer management container.

## Components

1. Docker Engine
   - Runs and manages containers.

2. Docker Compose
   - Defines and deploys multiple services.

3. Web Container 1
   - Runs the custom HTML application using Nginx.

4. Web Container 2
   - Runs the default Nginx application.

5. Portainer
   - Provides a graphical interface for managing containers.

## Architecture Flow

User
  |
  v
Docker Host
  |
  +---- Docker Engine
  |       |
  |       +---- Web Container 1
  |       |
  |       +---- Web Container 2
  |       |
  |       +---- Portainer
  |
  +---- Docker Compose
          |
          +---- Service Configuration

## Access Ports

- 8000: Custom application
- 8081: Nginx application
- 9443: Portainer dashboard
