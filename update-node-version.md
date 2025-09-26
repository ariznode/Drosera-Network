



# Update Operator
### 1. Download and install new release
```bash
cd ~
```
```bash
# Download
curl -LO https://github.com/drosera-network/releases/releases/download/v1.23.1/drosera-operator-v1.23.1-x86_64-unknown-linux-gnu.tar.gz

# Install
tar -xvf drosera-operator-v1.23.1-x86_64-unknown-linux-gnu.tar.gz
```
* Currently the Operator CLI version is `v1.23.1`. Verify the latest version [here](https://github.com/drosera-network/releases/releases)
* You have to get the link of `drosera-operator-v1.x.x-x86_64-unknown-linux-gnu.tar.gz`

Test the CLI with `./drosera-operator --version` to verify it's working.
```console
# Check version
./drosera-operator --version

# Move path to run it globally
sudo cp drosera-operator /usr/bin

# Check if it is working
drosera-operator --version
```

### 2. Install Docker image
```
docker pull ghcr.io/drosera-network/drosera-operator:latest
```

### 3. Head to Operator's directory:
```bash
cd ~
```
```bash
cd Drosera-Network
```

### 4. Stop Operator(s):
```bash
docker compose down -v
```

### 5. Restart Operator(s):
```bash
docker compose up -d
```

### 6. Node Logs:
```bash
docker compose logs -f
```
