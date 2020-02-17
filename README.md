# Python Port Forward
This script forwards a number of configured local ports to local or remote socket servers.

## Usage:
```
git clone git@github.com:vinodpandey/python-port-forward.git
cd python-port-forward

There are 2 ways to use this script
1. Command-line
2. Using config file


```

## Usage: Command-line
```
sudo python port-forward.py <local incoming port>:<dest hostname>:<dest port>

e.g. 
sudo python port-forward.py 80:localhost:8000

```

## Usage: Using config file
```
# update port-forward.config file
# default port forward is localhost:80 > localhost:8080 (80 localhost 8080)
sudo python port-forward.py

# with default port-forward.config, access: http://localhost/ -> this should now show content from http://localhost:8080/
# you can run a test python http server using below command to check the default configuration
# python -m SimpleHTTPServer 8080

```

## Configuration:
```
Add to the config file port-forward.config lines with contents as follows:

<local incoming port> <dest hostname> <dest port>
```

## Starting/stopping
```
Start the application at command line with 'sudo python port-forward.py' and stop the application by keying in <ctrl-c>.
```

## Errors
```
Error messages are stored in file 'error.log'.
```
