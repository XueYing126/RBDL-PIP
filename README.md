Python binding for PIP
============
To install the specific Python bindings for PIP/UIP/GIP, execute the following commands in your terminal:

```Bash
# Create and enter the project directory
mkdir RBDL
cd RBDL

# Clone the repository with all submodules
git clone --recursive https://github.com/XueYing126/RBDL-PIP.git

# Create a build directory
mkdir rbdl-build
cd rbdl-build/

# Configure the build
# Note: if this fails, run 'pip install cython'
cmake -D CMAKE_BUILD_TYPE=Release ../RBDL-PIP

# Compile the library
make
```
### Configure Environment

Add the following line to your ~/.zshrc file to allow Python to find the library (ensure you replace /path-to-folder/ with your actual directory path):

```Bash

export PYTHONPATH=$PYTHONPATH:/path-to-folder/RBDL/rbdl-build/python
```

