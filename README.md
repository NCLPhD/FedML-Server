# Installation
Installation user guide book: https://doc.fedml.ai/user_guide/open_source/installation.html

After the clone of this repository, please run the following command to get `FedML` submodule to your local.
```bash
cd FedML-Server/FedML
git submodule init
git submodule update
```


# Update FedML Submodule
```bash
cd FedML-Server/FedML
git checkout master && git pull
cd ..
git add FedML
git commit -m "updating submodule FedML to latest"
git push
```
