Things i forget and end up re googling. 

## apt-get package management

```bash
# Update the local pkg info
sudo apt-get update

# Upgrade all packages
#
# Below is an excerpt from man apt-get. Using upgrade keeps to the rule: under
# no circumstances are currently installed packages removed, or packages not 
# already installed retrieved and installed. If that's important to you, 
# use apt-get upgrade. If you want things to "just work", you probably want
# apt-get dist-upgrade to ensure dependencies are resolved.
sudo apt-get update && time sudo apt-get dist-upgrade

# Upgrade a single package
sudo apt-get update && sudo apt-get install --only-upgrade <pkg>
```

## yarn (npm replacement)

```bash
# Add packages to project
yarn add <pkg>

# Add packages globally
yarn global add <pkg>

# Path to global packages (add this to your bash profile)
yarn bin 

# Choose which package to update
yarn upgrade-interactive
```