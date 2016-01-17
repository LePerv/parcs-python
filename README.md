# PARCS Python
## Installation
### Linux /Fedora/
1. Install python2, virtualenv
2. Create virtual environment with: ```virtualenv -p python2 py2-env``` and activate it: ```source py2-env/bin/activate```
3. Install dependencies with pip: zerorpc, py-cpuinfo, requests, flask
## Running
### Use start.py
#### Config file mode
python2 start.py -config path_to_config/conf.config
Config file example:
Master:
```
[Node]
master=True
port=8080
job_home=/home/mhodovaniuk/WorkSpace/MasterWork/parcs-py-project/master_jobs
```
Worker:
```
[Node]
master=False
port=8090
job_home=/home/mhodovaniuk/WorkSpace/MasterWork/parcs-py-project/worker1_jobs
[Master Node]
ip=localhost
port=8080
```
#### Command line arguments
Use ```python2 start.py -h``` for help

