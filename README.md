# Development Container for ROS 2 on Apple Silicon
This Dockerfile is designed to create a Docker container specifically for ROS 2 Humble, optimized for M1/M2 Macs (ARM64 architecture).

## Getting Started

### Prerequisites
- Docker installed on your M1/M2 Mac

### Setup Instructions

#### 1. **Install Docker for M1/M2 Mac**:
Follow the official Docker installation guide for ARM64-based Macs.
#### 2. **Build the Container**:
Run the build script to build Docker image and install all dependencies. This should take around 10-20 minutes. 

```bash
   ./build_container.sh
```

1. **Start the Container**:
Initiate the container with

```bash
   ./start_container.sh
```

4. **Commit Changes**:
Save the current state of the Docker container using

```bash
   ./stop_container.sh
```

5. **Access the Container**:
For terminal access, run

```bash
   ./attach_container.sh
```

   to use bash inside the Docker container.

6. **Desktop Environment**: 
   To use the KDE Plasma Desktop via xrdp, connect using an RDP client to `127.0.0.1` or `localhost`.

### Recommended RDP Clients

- **Windows App**:
  It supports sound playback. Use your Mac username as your user name and leave the password blank when asked for it.

These steps will guide you through setting up and using a ROS 2 Docker container on your M1/M2 Mac, including desktop access through RDP. Choose the Microsoft Remote Desktop for comprehensive functionality, including sound playback and full keyboard support.
