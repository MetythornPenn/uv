# UV : Fast Python Package Manager

## setup guide 


```bash 
uv init 

uv venv
source .venv/bin/activate
uv sync 

# for jupyter notebook
uv add ipykernel 

# run uv tool like black for code formatting
uvx black src/main.py

# export requirements.txt
uv export -o requirements.txt

# install latest version of a package
uv add requests

# install a specific version
uv add requests=2.1.2

# change the bounds of a package's constraints
uv add 'requests<3.0.0'

# Make a dependency platform-specific:
uv add 'requests; sys_platform="linux"' 


# adding optional dep
uv add pandas --optional plot excel

# convert an existing virtualenv project
pip freeze > requirements.txt
uv init .
uv pip install -r requirements.txt

```

## Resource
- [datacamp uv tutorial](https://www.datacamp.com/tutorial/python-uv)
- []()