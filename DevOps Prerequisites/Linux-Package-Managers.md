# Linux Package Managers

## APT (Advanced Package Tool) - Debian/Ubuntu:

- **Installation:** Pre-installed on Debian-based systems.
- **Commands:**
  - Update Package List: `sudo apt update`
  - Install a Package: `sudo apt install package-name`
  - Remove a Package: `sudo apt remove package-name`
  - Upgrade Packages: `sudo apt upgrade`

## YUM (Yellowdog Updater, Modified) - CentOS/RHEL:

- **Installation:** Pre-installed on Red Hat-based systems.
- **Commands:**
  - Update Package List: `sudo yum check-update`
  - Install a Package: `sudo yum install package-name`
  - Remove a Package: `sudo yum remove package-name`
  - Upgrade Packages: `sudo yum update`

## Pacman - Arch Linux:

- **Installation:** Pre-installed on Arch-based systems.
- **Commands:**
  - Update Package List: `sudo pacman -Sy`
  - Install a Package: `sudo pacman -S package-name`
  - Remove a Package: `sudo pacman -R package-name`
  - Upgrade System: `sudo pacman -Syu`

## ZYpp - openSUSE:

- **Installation:** Pre-installed on openSUSE systems.
- **Commands:**
  - Update Package List: `sudo zypper refresh`
  - Install a Package: `sudo zypper install package-name`
  - Remove a Package: `sudo zypper remove package-name`
  - Upgrade System: `sudo zypper up`

# macOS Package Manager

## Homebrew:

- **Installation:** [Homebrew Installation](https://brew.sh/)
- **Commands:**
  - Install a Package: `brew install package-name`
  - Remove a Package: `brew uninstall package-name`
  - Upgrade Packages: `brew upgrade`

# Windows Package Manager

## Chocolatey:

- **Installation:** [Chocolatey Installation](https://chocolatey.org/install)
- **Commands:**
  - Install a Package: `choco install package-name`
  - Remove a Package: `choco uninstall package-name`
  - Upgrade Packages: `choco upgrade all`

---

# Linux Package Management with RPM and YUM

## RPM (Red Hat Package Manager):

- **Purpose:**
  - RPM is a low-level package management system used for installing, uninstalling, upgrading, querying, and verifying software packages on a Linux system.
  - It is primarily focused on the packaging format and installation of individual packages.
- **Commands:**
  - Install a Package: `rpm -i package.rpm`
  - Remove a Package: `rpm -e package`
  - Query Information: `rpm -q package`
  - List Installed Packages: `rpm -qa`
  - Verify Package: `rpm -V package`

## YUM (Yellowdog Updater, Modified):

- **Purpose:**
  - YUM is a higher-level package management tool built on top of RPM.
  - It resolves dependencies, making it easier to manage software packages by automatically handling package installations, removals, and updates.
- **Commands:**
  - Update Package List: `yum check-update`
  - Install a Package: `yum install package`
  - Remove a Package: `yum remove package`
  - Upgrade System: `yum update`

In practice, it's recommended to use YUM for day-to-day package management on Red Hat-based systems due to its ease of use and dependency resolution capabilities.



# Managing Linux Services

## Start `httpd` Service:

```bash
sudo systemctl start httpd
```

## Stop `httpd` Service:

```bash
sudo systemctl stop httpd
```

## Check `httpd` Service Status:

```bash
sudo systemctl status httpd
```

## Configure `httpd` to Start on Boot:

```bash
sudo systemctl enable httpd
```

## Configure `httpd` not to Start on Boot:

```bash
sudo systemctl disable httpd
```

## Test Web Server with `curl`:

```bash
curl http://localhost
```

## Reload Systemd Daemon After Modifying Unit Files:

```bash
sudo systemctl daemon-reload
```

# Docker Service Unit Files

## `docker.service` Unit File:

- Defines how the Docker daemon should run as a service.

## `docker.socket` Unit File:

- Defines the Docker socket activation.

## `docker-install.service` Unit File:

- Custom service file related to Docker installation or specific configurations.

# Example Usage for Docker Service:

```bash
# Start Docker Service
sudo systemctl start docker

# Stop Docker Service
sudo systemctl stop docker

# Check Docker Service Status
sudo systemctl status docker

# Enable Docker to Start on Boot
sudo systemctl enable docker

# Disable Docker from Starting on Boot
sudo systemctl disable docker

# Reload Systemd Daemon After Modifying Docker Unit Files
sudo systemctl daemon-reload
```

These commands are based on a systemd-based system. Adjustments may be needed based on specific system configurations and service names. Always refer to official documentation or manual pages (`man`) for detailed information on each command and service.