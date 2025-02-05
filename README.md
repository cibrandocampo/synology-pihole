# Pi-hole on Synology with Docker Compose  

This repository provides a **Docker Compose** configuration for running **Pi-hole** on a **Synology NAS** using the **Container Manager** application. **Pi-hole** is a network-wide ad blocker that functions as a **DNS sinkhole**, preventing ads and trackers from reaching your devices.  

## Prerequisites  

Before proceeding, ensure you have:  

- A **Synology NAS** with **DSM 7.0 or later** installed.  
- The **Container Manager** application installed and running.  

## Configuration & Customization  

To customize Pi-hole’s configuration, edit the `.env` file before importing the project into **Container Manager**. This allows you to tailor the container's settings to your specific needs.  

## Installation  

Follow these steps to deploy Pi-hole using **Docker Compose** on your Synology NAS:  

1. **Copy project files**:  
   Copy the `docker-compose.yml` and `.env` files to a folder on your **Synology NAS**. This can be done via SSH, the file manager, or any preferred method.  

2. **Open Container Manager**:  
   - Launch the **Container Manager** application from the **DSM** interface.  
   - Click **"Import"** to create a new project from Docker Compose files.  

3. **Select project files**:  
   - Browse to the folder where you copied the `docker-compose.yml` and `.env` files.  
   - Select the `docker-compose.yml` file and click **"Next"**.  

4. **Review settings**:  
   - The **Container Manager** will automatically detect the associated `.env` file and load environment variables.  
   - Review the imported configurations and make any necessary adjustments.  

5. **Deploy Pi-hole**:  
   - Click **"Apply"** to start the deployment.  

6. **Access the Pi-hole web interface**:  
   - Open a web browser and navigate to:  
     ```
     http://SYNOLOGY_IP:9003
     ```  
   - Replace `SYNOLOGY_IP` with your **Synology NAS’s local IP address**.  
   - Ensure the port matches the one defined in the `.env` file.  

7. **Complete setup**:  
   - Follow the Pi-hole setup wizard to configure DNS and ad-blocking preferences.  

## Troubleshooting & Contributions  

- If you encounter issues or have suggestions, feel free to reach out at **[hello@cibran.es](mailto:hello@cibran.es)**.  
- Contributions are welcome! Submit a **pull request** to improve this project.  

## License  

This project is licensed under the **[MIT License](LICENSE)**.