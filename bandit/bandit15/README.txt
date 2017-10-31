# Websites used for reference:
#
# https://blogcompsci.wordpress.com/2014/11/01/bandit-level-15-%e2%86%92-level-16/
#
#######################################################################################
#
# ssh -l bandit15 -p 2220 -L 1234:localhost:22 bandit.labs.overthewire.org
#
# The password for the next level can be retrieved by submitting the password of the current level to port 30001 on localhost using SSL encryption.
#
# openssl s_client -connect localhost:30001 -quiet < /etc/bandit_pass/bandit15
# Correct!
# cluFn7wTiGryunymYOu4RcffSxQluehd
#

