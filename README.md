## About
Python Notebook in Jupyter that will generate a series of unique images using a collection of layers.

## Getting Started
1. Install [Python](https://www.python.org/downloads/)
```
brew install python 
```

2. Look where python is installed
```
ls -l /usr/local/bin/python*
```
The output is something like this:
```
lrwxr-xr-x  1 arag0re  admin  34 Sep 01 16:32 /usr/local/bin/python3 -> ../Cellar/python/3.9.6/bin/python3
lrwxr-xr-x  1 arag0re  admin  41 Sep 01 16:32 /usr/local/bin/python3-config -> ../Cellar/python/3.9.6/bin/python3-config
lrwxr-xr-x  1 arag0re  admin  36 Sep 01 16:32 /usr/local/bin/python3.9 -> ../Cellar/python/3.9.6/bin/python3.9
lrwxr-xr-x  1 arag0re  admin  43 Sep 01 16:32 /usr/local/bin/python3.9-config -> ../Cellar/python/3.9.6/bin/python3.9-config
lrwxr-xr-x  1 arag0re  admin  37 Sep 01 16:32 /usr/local/bin/python3.9m -> ../Cellar/python/3.9.6/bin/python3.9m
lrwxr-xr-x  1 arag0re  admin  44 Sep 01 16:32 /usr/local/bin/python3.9m-config -> ../Cellar/python/3.9.6/bin/python3.9m-config
```

3. Change the default python symlink to the version you want to use from above. Note that, we only need to choose the one that end with python3.*.
```
ln -s -f /usr/local/bin/python3.9 /usr/local/bin/python
```

4. Check for installed python version
```
python --version
```
The output should be:
```
Python 3.9.6
```

5. Install PIP
```
sudo python -m ensurepip --default-pip
```

6. Update PIP
```
sudo python -m pip install --upgrade pip --user   
```

7. Install Python Pillow
```
python -m pip install pillow --user
```

8. Install Python display
```
python -m pip install display --user
```

9. Install Jupyter Notebook
```
python -m pip install jupyter --user
```

10. Add current PythonPath as PATH variable to .zshrc or .bashrc
```
export PATH=/Users/<username>/Library/Python/3.9/bin:$PATH
```

11. Run Jupyter in your nft-generator folder
```
jupyter notebook
```

12. Run the commands in [generate.ipynb] to generate images.

13. First time you run notebook, it will ask you to install ipykernel, accept this.
 
14. If the program executes successfully, it will output all the generated images to the /images folder, and the metadata to the /metadata folder. The filenames will refer to tokenIds. 
