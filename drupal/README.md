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

## Usage

- To stop the containers:
  ```bash
  docker-compose down
  ```

- To view logs:
  ```bash
  docker-compose logs -f
  ```

- To rebuild the containers after changes:
  ```bash
  docker-compose up --build
  ```

## Notes

- Ensure Docker and Docker Compose are installed on your system before proceeding.
- Update the `.env` file if custom configurations are required.
```

Let me know if you need further modifications!