# mariadb-master-slave-docker
This repository contains a Docker Compose setup for a MariaDB master-slave replication environment, including phpMyAdmin for easy database management.

## Overview

The setup consists of:

- **Master Database**: A MariaDB instance configured as the master for replication.
- **Slave Database**: A MariaDB instance configured as the slave that replicates data from the master.
- **phpMyAdmin for Master**: A web interface for managing the master database.
- **phpMyAdmin for Slave**: A web interface for managing the slave database.

## Prerequisites

- Docker
- Docker Compose

## Getting Started

1. **Clone the Repository**

   ```bash
   git clone https://github.com/ashokdevatwal/mariadb-master-slave-docker.git
   cd mariadb-master-slave-docker
   ```

2. **Configuration**

   - You can customize the MariaDB configuration files located in the `./master/my.cnf` and `./slave/my.cnf` directories. These files allow you to modify the MariaDB server settings.

3. **Starting the Services**

   Run the following command to start the services:

   ```bash
   docker-compose up -d
   ```

4. **Access phpMyAdmin**

   - Access the phpMyAdmin interface for the master database at [http://localhost:8081](http://localhost:8081) with the following credentials:
     - **Username**: `root`
     - **Password**: `root_password`
  
   - Access the phpMyAdmin interface for the slave database at [http://localhost:8082](http://localhost:8082) with the same credentials.

## Stopping the Services

To stop the services, run:

```bash
docker-compose down
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [Docker](https://www.docker.com/)
- [phpMyAdmin](https://www.phpmyadmin.net/)
- [MariaDB](https://mariadb.org/)
  
