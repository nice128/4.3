Installation
Run the script

wget https://raw.githubusercontent.com/saaiful/socks5/main/socks5.sh
sudo bash socks5.sh
You will be prompted for various options such as reconfiguring, adding users, or uninstalling the SOCKS5 server if it is already installed. During installation, you'll also be prompted for a username and password for the proxy authentication.

Testing the Proxy
The proxy can be tested from a Linux machine using curl. If you don't have curl installed, it can be installed with the following command:

apt-get install curl
Uninstallation
To completely remove the SOCKS5 server, select the Uninstall option when running the script. This will stop the service, remove the package, and clean up all related configuration and log files.

You can then test the proxy with:

curl -x socks5://username:password@proxy_server_ip:1080 https://ifconfig.me
curl -x socks5://username:password@proxy_server_ip:1080 https://ipinfo.io
