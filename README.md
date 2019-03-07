# nvOC easy-to-use Linux Nvidia Mining OS
Looking for Latest stable version? Go here: https://github.com/papampi/nvOC_by_fullzero_Community_Release/tree/release

## Community Edition - Quick start how-to
You can get nvOC running on your mining rig in some different ways:
- Picking and burning a pre-built whole disk OS image (recommended)
- Picking and burning a pre-built whole disk OS image targeting a beta testing branch
- Cloning this repo on existing OS installations

### Noob-proof: Pre-built images
Beta branches are not for noobs, become an insider and read below.

### For insiders: Pre-built images targeting beta/pre-release branches
Download the latest full nvOC OS image, then:
1. Write the image with your favourite HDD image writer of choicce
2. Browse to the small fat partition you can see on the drive. Download the latest nvOC configuration file named '1bash.template' from your branch of choice in this repo and save it there as '1bash'.
3. Edit this file with all your settings. The same file contains settings descriptions that will help you completing the setup.
4. Edit the firstboot.json file in that same folder and put your selected branch name in place of the default release branch.

### For experts: Clone this repo
You can find all files needed to run nvOC in this repo but it's recommended you run nvOC from inside a pre-built nvOC image for optimal support. You may have issues trying to setup nvOC from repo on generic Ubuntu or other Linux distro installations.
1. Create a folder in a nice place on your drive and clone this repo into it, we suggest '~/NVOC/mining' but you are free to choose

Starting from nvOC 2.1+ you can clone different versions of nvOC in different folders and keep all of them installed side-by-side for actual 'mining', 'testing' or other purposes. However a single running nvOC instance is supported: you cannot run multiple ones at the same time. Please, avoid cloning this repo directly into the user home directory

2. Setup your system to launch 2unix script from that folder on startup

Note that original nvOC startup method is based upon gnome-terminal default profile. You can switch, edit or disable this in termianl preferences. There is also a beta support for running nvOC as a systemd service.

3. Update the miners submodule

Just do 'git submodule update --init --remote miners', the correct git revision is automatically selected, which is the one linked to the nvOC tree you cloned.

4. Run the nvOC_miner_update.sh script to install the standard nvOC miner suite.

You can refer to https://github.com/papampi/nvOC_miners README for more help on how to update or enrich your miner collection in future

5. Edit nvOC configuration in 1bash file following contained instructions

## Download pre-built OS images

No pre-built image has been released for this dev branch, use one from the latest stable branch and follow instructions for insiders as described above.
