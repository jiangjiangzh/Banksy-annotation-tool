## Error when running ```npm install -g serve```

If the issue is due to the version of npm and node being too old, we need to update the version of NPM and Node

1. Download nvm
```shell
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.8/install.sh | bash
source ~/.nvm/nvm.sh
```
To check the installation, run the command line ```nvm``` . Note that if the response is something like ```-bash: nvm: command not found```, it indicates a failed installation.

2. Install Node and update NPM
```shell
nvm install 14.0.0
nvm install node    // install Node with latest version (v21.6.2)
npm install -g npm  // update NPM to latest version (10.2.4)
```
To check the installation of Node, run the command line ```node -v```.
To check the update of npm, run the command line ```npm -v```.

If the version of Node and NPM are the latest version, run the command line ```npm install -g serve``` again to install serve