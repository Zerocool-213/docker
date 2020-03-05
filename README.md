# Docker Compose for PyPlanet

Requirement : need to install docker, docker-compose and git. 

## Exemple to use

### 1. **Copy the git.**

On Linux, you can use this command to clone the git.
 
```bash
    git clone https://github.com/PyPlanet/docker.git
```

### 2. **Copy and edit environment variable.**

Go to docker folder.

```bash
    cd docker/
```

Copy environment file and rename in "dedicated_vars.env".

```bash
    cp dedicated_vars.default.env dedicated_vars.env
```
If you want change the server name or another variable, you can edit this file.

Use "vi" for edit your file.

```bash
    vi dedicated_vars.env
```

### 3. **Edit [base.py](https://github.com/PyPlanet/docker/blob/master/base.py) for change owner of the server.**

Change 'your-maniaplanet-login' for your login maniaplanet.

```bash
    vi base.py
```

### 4. finaly run your docker compose.

```bash
    docker-compose up
```

Or without logs.

```bash
    docker-compose up -d
```
