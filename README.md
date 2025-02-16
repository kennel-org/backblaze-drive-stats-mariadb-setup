# MariaDB my.cnf Samples for AlmaLinux 9

This repository provides sample MariaDB configuration files for AlmaLinux 9, designed to serve as a starting point for optimizing your database setup on specific hardware platforms. Please note that these configurations are provided as a baseline—customize them as needed for your own environment.

## Included Files

- **mycnf_lenovo.txt**  
  A sample configuration tailored for the **Lenovo ThinkCentre M75q Tiny Gen2**.

- **my.cnf_hp.txt**  
  A sample configuration tailored for the **HP EliteDesk 800 G4 DM**.

## Hardware Specifications

### Lenovo ThinkCentre M75q Tiny Gen2
- **Memory:** 64GB RAM  
- **Storage:** 2TB SSD  
- **CPU:** AMD Ryzen 5 PRO 5650GE with Radeon Graphics (6 cores, 12 threads)

### HP EliteDesk 800 G4 DM
- **Memory:** 64GB RAM  
- **Storage:** 2TB SSD  
- **CPU:** Intel® Core™ i5-8500T CPU @ 2.10GHz (6 cores)

## MariaDB Version Overview

These configurations have been tested with:
- **MySQL Ver 15.1 Distrib 10.5.27-MariaDB**
- **Platform:** Linux (x86_64)

## Installation

1. **Select the Appropriate Configuration**  
   Review the sample file that matches your hardware setup.

2. **Apply the Configuration**  
   Replace your current `/etc/my.cnf` with the content from the selected sample file.

3. **Restart MariaDB**  
   Apply the new configuration by restarting the MariaDB service:
   ```bash
   sudo systemctl restart mariadb
