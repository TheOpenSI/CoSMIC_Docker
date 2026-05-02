# Setup guide
1. Clone modular repo in your preferred folder on the machine:

```bash
### Linux/MacOS ###

# Using HTTPS (recommended for most users)
git clone https://github.com/TheOpenSI/COSMIC-DB.git CoSMIC_DB/
git clone https://github.com/TheOpenSI/CoSMIC.git
git clone https://github.com/TheOpenSI/CoSMIC_UI.git
git clone https://github.com/TheOpenSI/CoSMIC_Docker.git


# Using SSH (recommended if you've SSH keys configured)
git clone git@github.com:TheOpenSI/COSMIC-DB.git CoSMIC_DB/
git clone git@github.com:TheOpenSI/CoSMIC.git
git clone git@github.com:TheOpenSI/CoSMIC_UI.git
git clone git@github.com:TheOpenSI/CoSMIC_Docker.git
```

```ps1
### Windows ###

# Using HTTPS (recommended for most users)
git clone https://github.com/TheOpenSI/COSMIC-DB.git CoSMIC_DB/
git clone https://github.com/TheOpenSI/CoSMIC.git
git clone https://github.com/TheOpenSI/CoSMIC_UI.git
git clone https://github.com/TheOpenSI/CoSMIC_Docker.git


# Using SSH (recommended if you've SSH keys configured)
git clone git@github.com:TheOpenSI/COSMIC-DB.git CoSMIC_DB/
git clone git@github.com:TheOpenSI/CoSMIC.git
git clone git@github.com:TheOpenSI/CoSMIC_UI.git
git clone git@github.com:TheOpenSI/CoSMIC_Docker.git
```

2. Follow setup instructions in each repo (except part that build the compose file).

3. Spin up the unified compose file

> [!NOTE]
> It's possible to run Docker in rootless mode on Linux. However, the way to set
> it up is different on each Linux distros. Please refer to [this](https://docs.docker.com/engine/install) and [this](https://docs.docker.com/engine/security/rootless/)
> (all sourced from Docker documentation) to choose the one that fits for your
> current Linux distro.

```bash
# Linux/MacOS
sudo docker compose up --build -d # Refer to NOTE if running on rootless mode
```

```ps1
# Windows
docker compose up --build -d # Docker run through lightweight Linux VM on Windows so it's rootless by default
```

**The build process will take a while to fully up depending on your internet connection. Sit back, relax, and go do something else with your agents!**
