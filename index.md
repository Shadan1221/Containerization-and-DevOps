# Experiment 2: Docker Installation, Configuration and Running Images

## Aim

To install and configure Docker on the host system and understand Docker basics by pulling images, running containers, managing container lifecycle, and performing port mapping using Docker commands.

---


## Step 1: Verify Docker Installation

```bash
docker --version
```

**Output:**  
Docker version details are displayed, confirming successful installation.

---

## Step 2: Pull Nginx Image from Docker Hub

```bash
docker pull nginx
```

**Output:**  
The official Nginx image is downloaded successfully from Docker Hub.

---

## Step 3: Run Nginx Container

```bash
docker run -d -p 8081:80 nginx
```

**Explanation:**
* `-d` runs the container in detached mode  
* `-p 8081:80` maps host port 8081 to container port 80  
* `nginx` is the Docker image name  

---

## Step 4: List Running Containers

```bash
docker ps
```

**Output:**  
Displays container ID, image name, status, ports, and container name.

---

## Step 5: Access Nginx Web Server

Open browser and visit:

```text
http://localhost:8081
```

**Output:**  
The default *Welcome to nginx!* page is displayed.

---

## Step 6: Stop a Running Container

```bash
docker stop <container_id>
```

---

## Step 7: Remove a Container

```bash
docker rm <container_id>
```

---

## Step 8: List All Containers

```bash
docker ps -a
```

---

## Observations

| Feature | Observation |
|-------|------------|
| Image Download | Successful |
| Startup Time | Very fast |
| Resource Usage | Low |
| Port Mapping | Enabled browser access |
| Container Control | Easy using Docker CLI |

---

## Screenshots


### 1. Running Nginx Container

![Docker Run](screenshots/img1.png)

*Figure 1: Running Nginx container using Docker run command.*

---

### 2. Listing Running Containers

![Docker PS](screenshots/img2.png)

*Figure 2: Output of `docker ps` command.*

---

### 3. Nginx Running in Browser

![Nginx Browser](screenshots/img3.png)

*Figure 3: Nginx welcome page accessed via browser.*

---

### 4. Stopping and Removing Container

![Docker Stop](screenshots/img4.png)
![Docker Remove](screenshots/img5.png)

*Figure 4: Stopping and removing Docker container.*

---


## Result

Docker was successfully installed and configured. The Nginx image was pulled and executed as a container. All container management operations were performed successfully.

---

## Conclusion

Docker provides lightweight, fast, and efficient application deployment using containers. Compared to virtual machines, Docker containers offer better performance, reduced resource usage, and faster startup time.

---
