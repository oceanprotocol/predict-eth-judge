# predict-eth-judge

For judges of the predict-eth competition, a script to compute each submission's nmse.

To use: first do installation, then follow the CLI steps.

# Installation

Open a new terminal and:

```console
#clone repo
git clone https://github.com/oceanprotocol/predict-eth-judge.git
cd predict-eth-judge

#create a virtual environment
python -m venv venv

#activate env
source venv/bin/activate

#install dependencies
pip install wheel
pip install ocean-lib predict-eth ccxt enforce_typing numpy matplotlib

#add pwd to bash path
export PATH=$PATH:.

#set judges private key and Polygon Scan API Key
export REMOTE_TEST_PRIVATE_KEY1=<judges key>
export POLYGONSCAN_API_KEY=<api key>
```

# CLI

```text
Usage: pej getnmses START_DATE DEADLINE

Hard-coded values: NETWORK_NAME={NETWORK_NAME}, CHAINID={CHAINID}
Ennvars expected: REMOTE_TEST_PRIVATE_KEY1 (for judges' account) and POLYGONSCAN_API_KEY
```
