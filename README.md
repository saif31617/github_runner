### Download

# Create a folder
$ mkdir actions-runner && cd actions-runnerCopied!# Download the latest runner package
$ curl -o actions-runner-linux-x64-2.330.0.tar.gz -L https://github.com/actions/runner/releases/download/v2.330.0/actions-runner-linux-x64-2.330.0.tar.gzCopied!# Optional: Validate the hash
$ echo "af5c33fa94f3cc33b8e97937939136a6b04197e6dadfcfb3b6e33ae1bf41e79a  actions-runner-linux-x64-2.330.0.tar.gz" | shasum -a 256 -cCopied!# Extract the installer
$ tar xzf ./actions-runner-linux-x64-2.330.0.tar.gz


### Configure

sudo chown -R ubuntu:ubuntu /home/ubuntu/actions-runner

# Give full permissions
sudo chmod -R 755 /home/ubuntu/actions-runner

# Switch to ubuntu user if you're root
su - ubuntu

# Create the runner and start the configuration experience
$ ./config.sh --url https://github.com/saif31617/github_runner --token ALQJBP7DK73E4IHJVNOVSL3JL2Y7YCopied!# Last step, run it!
$ ./run.sh



ubuntu@ip-192-168-0-132:~/actions-runner$ ./config.sh --url https://github.com/saif31617/github_runner --token ALQJBP7DK73E4IHJVNOVSL3JL2Y7Y

--------------------------------------------------------------------------------
|        ____ _ _   _   _       _          _        _   _                      |
|       / ___(_) |_| | | |_   _| |__      / \   ___| |_(_) ___  _ __  ___      |
|      | |  _| | __| |_| | | | | '_ \    / _ \ / __| __| |/ _ \| '_ \/ __|     |
|      | |_| | | |_|  _  | |_| | |_) |  / ___ \ (__| |_| | (_) | | | \__ \     |
|       \____|_|\__|_| |_|\__,_|_.__/  /_/   \_\___|\__|_|\___/|_| |_|___/     |
|                                                                              |
|                       Self-hosted runner registration                        |
|                                                                              |
--------------------------------------------------------------------------------

# Authentication


√ Connected to GitHub

# Runner Registration

Enter the name of the runner group to add this runner to: [press Enter for Default]

Enter the name of runner: [press Enter for ip-192-168-0-132] saifullah

This runner will have the following labels: 'self-hosted', 'Linux', 'X64'
Enter any additional labels (ex. label-1,label-2): [press Enter to skip]

√ Runner successfully added

# Runner settings

Enter name of work folder: [press Enter for _work]

√ Settings Saved.
