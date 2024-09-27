# union_validator_node_guide

---

## Overview

This guide provides step-by-step instructions for setting up a node operator on the Union Build infrastructure. 

## Prerequisites

Before starting, ensure you have the following:

- A server with at least 4GB RAM and 2 CPU cores.
- A Linux-based operating system (Ubuntu recommended).
- Basic knowledge of command-line operations.
- An active Union Build account.

## Step 1: Server Setup

1. **Log into your server:**
   ```bash
   ssh user@your-server-ip
   ```

2. **Update your package list and install necessary dependencies:**
   ```bash
   sudo apt update && sudo apt upgrade -y
   sudo apt install -y curl git
   ```

## Step 2: Install Node Software

1. **Clone the Node Repository:**
   ```bash
   git clone https://github.com/UnionBuild/node-repo.git
   cd node-repo
   ```

2. **Install the Node:**
   ```bash
   ./install.sh
   ```

## Step 3: Configuration

1. **Edit the configuration file:**
   ```bash
   nano config.yaml
   ```
   - Set your node's parameters (e.g., port, network ID).

2. **Start the Node:**
   ```bash
   ./start-node.sh
   ```

## Step 4: Monitoring

- Use the following command to check the node status:
  ```bash
  ./status.sh
  ```

## Step 5: Troubleshooting

If you encounter issues, refer to the logs:
```bash
tail -f logs/node.log
```

## Conclusion

You have successfully set up your node operator on the Union Build infrastructure. For more information, visit the [Union Build Documentation](https://docs.union.build).

---

