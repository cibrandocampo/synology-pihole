# Pi-hole on Synology with Docker Compose

This repository contains a Docker Compose file to run Pi-hole on a Synology NAS using the Container Manager application. Pi-hole is a network-wide ad blocker that acts as a DNS sinkhole, blocking ads and trackers before they reach your devices.

## Prerequisites

- A Synology NAS with DSM > 7.0 installed and properly configured.
- The Synology Container Manager application installed and running.

## Configuration/Customization

If you need to modify the configuration of the Unifi Controller, you can edit the `.env` file you copied to the NAS before importing the project into the Container Manager. This allows you to customize the container's behavior according to your specific requirements.

## Installation

1. Copy the `docker-compose.yml` and `.env` files to a folder on your Synology NAS. You can do this using the command line, file manager, or any other preferred method.

2. Open the Synology Container Manager application from the DSM desktop.

3. In the Container Manager, click on "Import" to create a new project from your Docker Compose files.

4. Browse to the folder where you copied the `docker-compose.yml` and `.env` files.

5. Select the `docker-compose.yml` file and click "Next."

6. The Container Manager will automatically detect the `.env` file associated with the Docker Compose and load the environment variables.

7. Review the settings and configurations imported from the `docker-compose.yml` and `.env` files. Make any necessary adjustments if needed.

8. Click "Apply" to start the deployment of Pi-hole based on the provided settings.

9. Once the container is deployed, access the Pi-hole web interface through your web browser: http://SYNOLOGY_IP:9003

Replace `SYNOLOGY_IP` with the local IP address of your Synology, and use the port configure in the `.env` file.

10. Follow the Pi-hole setup wizard to configure your DNS and ad-blocking preferences.

## Issues and Contributions

If you encounter any problems or have any suggestions, feel free to contact me via (hello@cibran.es). You can also contribute to improving this project by submitting pull requests.

## License

This project is licensed under the [MIT License](LICENSE).
