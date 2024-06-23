This Code simply blocks the websites mentioned in the input the path of the hosts file ie., hosts_path. You have to create a new folder and specify the path in the main.py. Otherwise it will give an error of - 

" FileNotFoundError: [Errno 2] No such file or directory: '/etc/hosts'" 

Important Notes:

Run as root: This script modifies the /etc/hosts file, which requires root privileges. Make sure to run this script with appropriate permissions.

Timing: The script uses a sleep interval of 5 seconds, which means it checks and updates the hosts file every 5 seconds.

Operating System: The path to the hosts file (/etc/hosts) is for Unix-like operating systems (Linux, macOS). For Windows, the path is typically C:\Windows\System32\drivers\etc\hosts. Adjust the hosts_path variable accordingly if running on a different OS.