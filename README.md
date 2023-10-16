# C.O.P
# HTB COP web challege
# To win this challenge First you need to run burp suite and intercept the traffic
# sent the traffic to repeater
# we can used ' OR id='1 sql inject for the url but before pasting it in the get request you need to encode it using urlencode
# on the get it going to look like this when yoy finish the above:   GET /view/%27%20OR%20id%3D%271 HTTP/1.1
# now used the exploit.py code to get the payload and used it with 'UNION SELECT' before the start of payload but remember to encode it first using urlencode
# eg: GET /view/'UNION SELECT'{payload} but encode first the union select along with the payload
