# Python Virtual Environments

## What is a virtual environment

A Python virtual environment is an isolated runtime environment that allows you
to run applications and programs in that environment so you don't interfere with
applications or programs on the same system.

When the `venv` tool is run, a directory is created with all the necessary files
to run Python in an isolated system. When you work in the environment and
install other packages or libraries, they are stored in the same directory.

In our case, this will allow us to work in the same environment without having
to wonder if there are differences between our systems.

## How to create a virtual environment

There is already a virtual environment in the code base, so it doesn't need to
be done again.

If another one is needed to be made, use the following command in a PowerShell
terminal with your location set to the root of the project:

```powershell
python3 -m venv flappyBird-env
```

## Using the virtual environment

To use the environment, all you will need to do is dot-source a script the
virtual environment provides.

dot-sourcing is a method in PowerShell to run a script and have it act as if
it's in your current session. the syntax is simple. It's just a period (`.`)
followed by a space and a file path. Make sure your PowerShell terminal location
is set to the root of the Flappybird project.

```powershell
. /flappybird-env/bin/Activate.ps1
```

This should start the virtual environment and your terminal prompt will have an
indication saying so.

## Issues

If there are any problems, create a new issue and we will resolve it. 
