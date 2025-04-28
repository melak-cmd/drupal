```markdown
# Drupal

## Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd drupal
   ```

2. Build and start the Docker containers:
   ```bash
   docker-compose up -d
   ```

3. Access the Drupal site:
   - Open your browser and navigate to `http://localhost`.

4. Follow the Drupal installation wizard to complete the setup.

# PlantUML Server

This project sets up a PlantUML server using Docker.

## Prerequisites

- Docker installed on your system
- Docker Compose installed

## Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd planttext-server
   ```

2. Start the PlantUML server:
   ```bash
   docker-compose up -d
   ```

3. Access the PlantUML server:
   - Open your browser and navigate to `http://localhost:8080`.

## Usage

- To stop the server:
  ```bash
  docker-compose down
  ```

- To view logs:
  ```bash
  docker-compose logs -f
  ```

- To restart the server:
  ```bash
  docker-compose restart
  ```

## Configuration

- The server runs on port `8080` by default. You can change this in the `docker-compose.yml` file under the `ports` section:
  ```yaml
  ports:
    - "8080:8080"
  ```

- Resource limits are set as follows:
  - CPU: `0.5`
  - Memory: `1024M`

  You can adjust these values in the `deploy.resources.limits` section of the `docker-compose.yml` file.

## Notes

- This setup uses the `plantuml/plantuml-server:jetty` image.
- Ensure that port `8080` is not in use by other applications on your system.
```