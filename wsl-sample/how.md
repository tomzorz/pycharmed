## pycharming

Useful pycharm + wsl + windows thingamajigs.

## Windows Setup

In admin powershell, enable access to WSL via the firewall:

```powershell
New-NetFirewallRule -DisplayName "WSL" -Direction Inbound  -InterfaceAlias "vEthernet (WSL)"  -Action Allow
```

## WSL Setup

1. Install conda
2. Setup conda env(s)
3. Place `pythonconda` into home directory

## Conda things

Created env via:

`conda create --name ENVNAME python=3.9`

To list envs:

`conda info --envs`

To activate the new env:

`conda activate ENVNAME`

To return to base: 

`conda activate`

To search / install / list packages:

`conda search tqdm`

`conda install tqdm`

`conda list`

## Pycharm things

Set up a new python interpreter via File > Settings > Project: YOURPROJECT > Python Interpreter > + Button

- Select your WSL setup
- Select your /home/username/pythonconda file

