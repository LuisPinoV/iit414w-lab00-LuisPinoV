# iit414w-lab00-LuisPinoV

# Header
Luis Nicolas Pino Velasquez, LuisPinoV, IIT414W, 11/03/2026

# System Info

OS: linux, Ubuntu 24.04.4 LTS
Python: python3 3.12.3
pip: 24

# Setup instruccions and how to run

Some Ubuntu distribuitions have python3 already installed but in windows it requieres you to install python3
In case you need it, here are the CMD commands to install it in each OS

To run them you need to open a terminal in the same folder of the repository

    Ubuntu: sudo apt install python3

    Windows: winget install Python.Python.3

Then you need to create a virtual enviroment to run the nootebooks
To create it run the following command

    python3 -m venv .venv

it will create a enviroment called ".venv" in the same folder you are on
Then you have to run the requirements to intall everything you need to run these nootebooks
You can run the requirements whith the following command

    pip install -r requirements.txt

Now you can run the nootebooks, press in run all. If ask you to install ipkernell press "Accept"


# Problems encountered: 
PermissionError: [Errno 13] Permission denied: '/home/data'

cache_path = os.path.join(os.path.dirname(os.getcwd()),'', 'data', 'fastf1_cache') -> cache_path = os.path.join(os.path.dirname(os.getcwd()), 'data', 'fastf1_cache')

It happend because ubuntu dont give permision to access to root folders (and with reason) to fix it i change the location of the folder to: 

cache_path = os.path.join(os.path.dirname(os.getcwd()), 'data', 'fastf1_cache') -> cache_path = os.path.join(os.path.dirname(os.getcwd()), 'data', 'fastf1_cache')

Thats the only real problem i encounter during this excercise

# Expected outputs

Most expected outputs are messages that show the information requested with an explanation and tables to show more "advance" data