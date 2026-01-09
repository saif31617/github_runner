# chat application EC2 Based CICD via Github

### **Note : Change the user to ubuntu**

#### step 1 : Create a folder

$ mkdir actions-runner && cd actions-runner

#### step 2 : Download the latest runner package

$ curl -o actions-runner-linux-x64-2.330.0.tar.gz -L https://github.com/actions/runner/releases/download/v2.330.0/actions-runner-linux-x64-2.330.0.tar.gz

#### step 3 :Validate the hash

$ echo "af5c33fa94f3cc33b8e97937939136a6b04197e6dadfcfb3b6e33ae1bf41e79a  actions-runner-linux-x64-2.330.0.tar.gz" | shasum -a 256 -c

####  step 4 : Extract the installer

$ tar xzf ./actions-runner-linux-x64-2.330.0.tar.gz


#### step 5 : Create the runner and start the configuration experience
$ ./config.sh --url https://github.com/saif31617/github_runner --token <Get Token from Github-settings/actions/runners>

#### Last step, run it!
$ ./run.sh


