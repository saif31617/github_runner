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
