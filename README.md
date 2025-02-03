# Jenkins-Script Repository

This repository contains a shell script designed to automate the installation and setup of Jenkins on a Linux system.

## Script Details

- **jenkins.sh**: A shell script that automates the following tasks:
  - Installs Java Development Kit (JDK), a prerequisite for Jenkins.
  - Adds the Jenkins repository to the system's package manager.
  - Installs Jenkins.
  - Starts and enables the Jenkins service to run on system boot.
  - Provides instructions to retrieve the initial admin password for Jenkins setup.

## Usage

To execute the script:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/MorielMauni/Jenkins-Script.git
   cd Jenkins-Script
   ```

2. **Run the Script**:
   ```bash
   chmod +x jenkins.sh
   sudo ./jenkins.sh
   ```

   *Note*: Ensure you have sufficient privileges to install packages and start services.

3. **Post-Installation**:
   - After the script completes, Jenkins will be accessible via `http://your_server_ip_or_domain:8080`.
   - Retrieve the initial admin password using:
     ```bash
     sudo cat /var/lib/jenkins/secrets/initialAdminPassword
     ```
   - Follow the on-screen instructions to complete the Jenkins setup.

## Prerequisites

- A Linux-based operating system.
- Sudo privileges for package installation and service management.
- Internet connectivity to download packages.

## Contributing

Contributions are welcome! If you'd like to enhance the script or add new features:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Commit your changes with descriptive messages.
4. Submit a pull request for review.

Please ensure your contributions align with the existing coding style and include necessary documentation.

## Contact

For any questions or issues, feel free to reach out via email: morielmauni@gmail.com
