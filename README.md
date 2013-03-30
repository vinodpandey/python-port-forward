python-port-forward
===================

Usage: 
git clone git@github.com:vinodpandey/python-port-forward.git


# This script forwards a number of configured local ports
# to local or remote socket servers.
#
# Configuration:
# Add to the config file port-forward.config lines with
# contents as follows:
#   <local incoming port> <dest hostname> <dest port>
#
# Start the application at command line with 'sudo python port-forward.py'
# and stop the application by keying in <ctrl-c>.
#
# Error messages are stored in file 'error.log'.
