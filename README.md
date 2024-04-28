**Hyprdots Installation Guide**

Welcome to Hyprdots! Below are the steps to get started with installing and setting up Hyprdots on your system.

### Step 1: Download Hyprdots

First, you need to download the base Hyprdots from the official repository.

Repository Link: [Hyprdots Repository](https://github.com/prasanthrangan/hyprdots)

```bash
git clone --depth 1 https://github.com/prasanthrangan/hyprdots ~/Hyprdots
```

### Step 2: Install Dependencies

Ensure you have Git installed on your system. If not, you can install it using pacman.

```bash
sudo pacman -Sy git
```

### Step 3: Run Installation Script

Navigate to the Hyprdots directory and run the installation script.

```bash
cd ~/Hyprdots/Scripts
./install.sh
```

### Step 4: Configure Hyprdots

Congratulations! You're now in Hyprland. To further customize your environment, follow the additional steps below.

#### Updating Package List

To get the package list of your device, you can regularly update `package_list.txt` with the apps you use. Then, run the following commands to install the packages.

```bash
sudo pacman -S --needed - < package_list.txt
```

If you use yay, you can also install packages from `yay_packages.txt`.

```bash
yay -S --needed - < yay_packages.txt
```

