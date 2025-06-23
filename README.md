<div align="center">

  # Born2beroot Project

  <p align="center"><a href="https://github.com/aabdulmecitz/42-Born2beroot" target="_blank"><img align="center" alt="born2beroot" src="https://github.com/mcombeau/mcombeau/blob/main/42_badges/born2berootm.png?raw=true"> </a></p>

  [![forthebadge](https://forthebadge.com/images/badges/made-with-c.svg)](https://forthebadge.com)
  [![forthebadge](https://forthebadge.com/images/badges/built-with-love.svg)](https://forthebadge.com)

   <a img src="https://img.shields.io/badge/score-125%20%2F%20100-success?style=for-the-badge"/></a>
   <a img src="https://img.shields.io/badge/circle-2-magenta?style=for-the-badge"/></a>
   <a img src="https://img.shields.io/badge/42-Evaluation-red?style=for-the-badge"/></a>

  <p align="center"><a href="https://https://42istanbul.com.tr/" target="_blank"><img src="https://img.shields.io/static/v1?label=&message=Istanbul&color=000&style=for-the-badge&logo=42""></a></p>

  <p align="center">125/100 :white_check_mark:</p>
</div>

This project aims to set up a virtual machine and install a Debian server with specific services.

## Mandatory Part

The mandatory part of the project includes:

*   **Virtual Machine Setup**:
    *   Choose a virtualization software (VirtualBox or KVM).
    *   Install a Debian or CentOS server.
    *   The server must not have a graphical interface.
*   **Disk Partitioning**:
    *   Create at least 4 encrypted partitions using LVM.
*   **Services**:
    *   **SSH**: The SSH service must run on a port other than 22. It should not be possible to log in as root via SSH.
    *   **UFW (Uncomplicated Firewall)**: The firewall must be configured to allow only the necessary ports for the services.
    *   **Hostname**: The hostname of the machine must be your login followed by `42` (e.g., `jdoe42`).
*   **User Management**:
    *   Create a user with your login.
    *   This user must be part of the `sudo` and `user42` groups.
    *   The `root` password must be changed.
    *   A strong password policy must be implemented.
*   **Scripting**:
    *   Write a script named `monitoring.sh` that displays information about the server every 10 minutes when a user logs in. The script should show:
        *   The architecture of the operating system and its kernel version.
        *   The number of physical processors.
        *   The number of virtual processors.
        *   The current available RAM on the server and its utilization rate (as a percentage).
        *   The current available memory on the server and its utilization rate (as a percentage).
        *   The current utilization rate of the processors (as a percentage).
        *   The date and time of the last reboot.
        *   Whether LVM is active.
        *   The number of active connections.
        *   The number of users using the server.
        *   The IPv4 address of the server and its MAC (Media Access Control) address.
        *   The number of commands executed with the `sudo` program.

## Bonus Part

The bonus part of the project includes:

*   **WordPress Setup**:
    *   Set up a functional WordPress website with the following services:
        *   `nginx`
        *   `PHP`
        *   `MariaDB`
*   **Additional Services**:
    *   **FTP Service**: Set up a secure FTP service (vsftpd) jailed to the user's home directory.
    *   **An additional service of your choice**: For example, a web-based management tool like `Webmin`.