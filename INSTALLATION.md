# FFTrack Installation Guide

This guide will walk you through the steps required to install FFTrack on your system. FFTrack is a music recognition tool that allows you to identify songs from audio input, and it works on Linux, macOS, and Windows operating systems.

## Prerequisites
Before you begin the installation, ensure that you have Python installed on your system. FFTrack requires Python 3.9 or higher. You can check your Python version by running:
```bash
python --version
```
or
```bash
python3 --version
```
If Python is not installed or you need to upgrade to a newer version, visit [Python's official website](https://www.python.org/downloads/) for download and installation instructions.

## Step-by-Step Installation

### Linux (Ubuntu)
1. **Update and Install Dependencies**:
   Open your terminal and run the following command to update your package list and install necessary dependencies:
   ```bash
   sudo apt-get update && sudo apt-get install -y portaudio19-dev
   ```

2. **Set Up Python Environment**:
   It's recommended to use a virtual environment to avoid conflicts with system-wide packages. If `venv` is not installed, you can install it with:
   ```bash
   sudo apt-get install python3-venv
   ```
   Then, create and activate a virtual environment:
   ```bash
   python3 -m venv fftrack-env
   source fftrack-env/bin/activate
   ```

3. **Install FFTrack**:
   With the virtual environment activated, install FFTrack using pip:
   ```bash
   pip install fftrack
   ```

### macOS
1. **Install Dependencies**:
   First, ensure you have Homebrew installed by running `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`. Then, install PortAudio using Homebrew:
   ```bash
   brew install portaudio
   ```

2. **Set Up Python Environment**:
   Create and activate a virtual environment in your preferred directory:
   ```bash
   python3 -m venv fftrack-env
   source fftrack-env/bin/activate
   ```

3. **Install FFTrack**:
   With your environment activated, install FFTrack via pip:
   ```bash
   pip install fftrack
   ```

### Windows
1. **Install Dependencies**:
   Download and install PortAudio from [PortAudio's official page](http://www.portaudio.com/download.html). Ensure that the PortAudio binaries are in your system's PATH.

2. **Set Up Python Environment**:
   Open Command Prompt or PowerShell and set up a virtual environment:
   ```bash
   python -m venv fftrack-env
   .\fftrack-env\Scripts\activate
   ```

3. **Install FFTrack**:
   Finally, install FFTrack using pip:
   ```bash
   pip install fftrack
   ```

## Verifying the Installation
To verify that FFTrack has been installed correctly, you can run:
```bash
fftrack --help
```
This command should display the help message for FFTrack, confirming that it is installed correctly and ready to use.

## Troubleshooting
If you encounter any issues during the installation, please ensure that:
- You have the correct permissions to install software on your system.
- Your internet connection is stable during the download of FFTrack and its dependencies.
- Python and pip are correctly installed and updated to their latest versions.

For specific errors, refer to the error messages guide provided in the FFTrack documentation or seek help from the FFTrack support team.

With FFTrack installed, you are now ready to start identifying songs directly from your terminal!