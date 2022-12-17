***Secure Personalized Federated Learning***

**MP-SPDZ Installation (macOS)**
(Perform these commands starting from spfl directory)

```
git clone https://github.com/data61/MP-SPDZ.git
cd MP-SPDZ

Scripts/tldr.sh
./compile.py tutorial

echo 1 2 3 4 > Player-Data/Input-P0-0
echo 1 2 3 4 > Player-Data/Input-P1-0
Scripts/mascot.sh tutorial
```
If commands run without failure and tutorial runs succesfully then the installation should be good.

**Python Environment Setup**
Ensure you are using Python-3.8 or Python-3.9 (Pytorch does not support later versions) Also create a new Python virtual environment to avoid dependency conflicts (conda or venv is suggested) and install the requirements.

Virtual Environment Creation and Setup (Using venv)
```
# Make sure to run from spfl directory
python3 -m venv venv
source venv/bin/activate
pip3 install -r requirements.txt
```

Confirm all libraries are installed successfully. Note: You may need to upgrade pip before running pip3 install.

**Code Execution**
```
MP-SPDZ/compile.py <filename>.mpc
Scripts/mascot.sh <filename>
```

To run on protocols other than mascot, follow instructions at: https://mp-spdz.readthedocs.io/en/latest/readme.html#dishonest-majority
