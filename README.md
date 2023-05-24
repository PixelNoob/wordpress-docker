# WordPress Docker

This repository provides a Docker Compose configuration for running a WordPress website using MySQL, WordPress, and Nginx.

## Prerequisites

Before getting started, ensure that you have Docker and Docker Compose installed on your system.

## Usage

1. Clone this repository to your local machine:

   ```shell
   git clone https://github.com/PixelNoob/wordpress-docker
   ```

2. Navigate to the cloned repository:

   ```shell
   cd wordpress-docker
   ```

3. Customize the environment variables:

   - Rename the `.env.example` file to `.env`.
   - Open the `.env` file and update the variables according to your requirements.

4. Start the WordPress environment:

   ```shell
   docker-compose up -d
   ```

   This command will create and start the MySQL, WordPress, and Nginx containers in the background.

5. Access the WordPress website:

   Open your web browser and visit [http://localhost](http://localhost) to access your WordPress site.

6. Clean up:

   To stop and remove the containers, run:

   ```shell
   docker-compose down
   ```

## Configuration

The Docker Compose configuration consists of the following services:

- **db**: MySQL database service for storing WordPress data.
- **wordpress**: WordPress service based on the official WordPress image.
- **webserver**: Nginx service for serving the WordPress site.
- **certbot**: Create a letsencrypt certificate for your domain (Its commented as is not needed for local development).

You can customize the configuration by modifying the `docker-compose.yml` file.

## Contributing

Contributions are welcome! If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request.
