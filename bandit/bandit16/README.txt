# Websites used for reference:
#
# https://blogcompsci.wordpress.com/2014/11/01/bandit-level-16-%e2%86%92-level-17/
#
#######################################################################################
# ssh -l bandit16 -p 2220 -L 1234:localhost:22 bandit.labs.overthewire.org

# nmap -p 31000-32000 localhost
# The above will scan port ranges from 31000 to 32000 on localhost 

# This led to following: 
# 
# 31046/tcp open  unknown
# 31518/tcp open  unknown
# 31691/tcp open  unknown
# 31790/tcp open  unknown
# 31960/tcp open  unknown
# 
#
# cat /etc/bandit_pass/bandit16 | openssl s_client -connect localhost:31518 -quiet > /tmp/key/b16pkey
# cat /etc/bandit_pass/bandit16 | openssl s_client -connect localhost:31046   -quiet > /tmp/key/b16pkey
# cat /etc/bandit_pass/bandit16 | openssl s_client -connect localhost:31790   -quiet > /tmp/key/b16pkey
# chmod 600 /tmp/key/b16pkey
