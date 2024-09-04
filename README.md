Ping Multiple IPs Script
This Python script automates the process of pinging multiple IP addresses. It reads the IP addresses from an Excel file, pings each one, and then reports whether each IP is reachable or not.

Features
Automated IP Ping: The script automates the process of pinging a list of IP addresses.
Excel Integration: IP addresses are read from an Excel file, making it easy to manage the list of IPs.
Reachability Check: The script checks the reachability of each IP and outputs the result.
Prerequisites
Before running the script, make sure you have the following installed:

Python 3.x
Required Python packages: pandas, openpyxl (for reading Excel files)
You can install the necessary packages using pip:

sh
Copy code
pip install pandas openpyxl
Usage
Prepare the Excel File: Create an Excel file (ping_multiple_ips.xlsx) with the following structure:

Sheet Name: ip_addresses (or change the sheet_name variable in the script)
Column Name: IP (or change the column_name variable in the script)
The column should contain the IP addresses you want to ping.

Run the Script:

sh
Copy code
python ping_multiple_ips.py
The script will read the list of IP addresses from the Excel file, ping each one, and print whether each IP is reachable or not.

Customization
Ping Command: The script uses the default ping command available on your system. If you're running the script on a non-Windows platform, you may need to adjust the ping_ip function to match the expected output format.
Timeout and Packet Settings: If you need to adjust the number of packets or timeout settings, modify the subprocess.check_output command within the ping_ip function.
Contribution
Contributions are welcome! Feel free to fork this repository, submit pull requests, or open issues for any bugs or feature requests.

License
This project is licensed under the MIT License. See the LICENSE file for details.
