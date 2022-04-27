# Installation
Installation user guide book: https://doc.fedml.ai/user_guide/open_source/installation.html

pip install -r requirements.txt

## Problem solutions
**ERROR: Failed building wheel for mpi4py**
If you get an error about `ERROR: Could not build wheels for mpi4py which use PEP 517 and cannot be installed directly`
Please make sure your host already installed `libopenmpi-dev`
```bash
# Example command for libopenmpi-dev installation.
sudo apt install libopenmpi-dev 
```

# Prepare Dataset
```
cd FedML/data/MNIST/
sh download_and_unzip.sh
cd ../../../
```

# Launch the HTTP Server
Set the server IP and port and then run the following script:
```
python app.py
```

# Preprocess Dataset
```
cd executor
sh server_start.sh
```

# Launch the mobile device simulator
```
cd client_simulator
python3 ./client_simulator/mobile_client_simulator.py --client_uuid '0'
```
