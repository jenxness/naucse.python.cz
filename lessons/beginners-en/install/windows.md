# Python installation for Windows 

Go to [the Python website](https://www.python.org/downloads/) and 
download the latest stable version of Python. From version 3.6.0.
there are some enhancements for Windows so download only version
 **3.6.0 and above**.

How to know which installer is the right one?
If your computer has 64bit Windows then download *Windows x86-64 executable installer*.
If your Windows is only 32bit download *Windows x86 executable installer*.


> [note]
> If you don't know what Windows version do you have just open **Start**, 
> search **System** and open **System information**.
>
> {{ figure(
    img=static('windows_32v64-bit.png'),
    alt='Windows version',
) }}

Then you can run the installer.
In the beginning check **Install launcher for all Users**
and also **Add Python 3.6 to PATH**.
This will make creating venv much easier.

(If you don't have admin rights don't check *Install launcher for all Users*.)

{{ figure(
    img=static('windows_add_python_to_path.png'),
    alt='Python installation',
) }}

Then click **Install now** and follow the instructions.

If you have your command line open, close it and open again.

## conda installation

For conda installation use [this link](https://docs.conda.io/projects/conda/en/latest/user-guide/install/windows.html) and choose Anaconda.

Then you have to add full path to C:\\.......\Continuum\anaconda3\Scripts (instead of
dots there will be something different regarding where you installed it) to your 
environment variable PATH - try to find out by yourself (but if you will have some 
troubles contact us). You will know that it's been added successfully by typing into 
your command line:

```bash
conda --help
``` 

After succesfull installation follow how to [create virtual environment](https://conda.io/docs/user-guide/tasks/manage-environments.html)

