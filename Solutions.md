## Solution 1

I just removed the class ACM_Debugging_Competition and removed those unnecessary functions for hi and bye and forked it. Also in the import line, I just imported flask, the other things like url_request for redirect were useless. Also, I changed the port number in the app.run(), because that was when it worked in sandbox

##Solution 2

I changed this line from 
 mapped_key = sorted_keys[(index + len(sorted_keys)) % len(services_name)]

to

 mapped_key = sorted_keys[(index + len(sorted_keys)) % len(services_map)]
