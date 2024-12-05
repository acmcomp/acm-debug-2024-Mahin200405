## Solution 1

I just removed the class ACM_Debugging_Competition and removed those unnecessary functions for hi and bye and forked it. Also in the import line, I just imported flask, the other things like url_request for redirect were useless. Also, I changed the port number in the app.run(), because that was when it worked in sandbox

## Solution 2

I changed this line from
```Python
 mapped_key = sorted_keys[(index + len(sorted_keys)) % len(services_name)]
```

to
```Python
 mapped_key = sorted_keys[(index + len(sorted_keys)) % len(services_map)]
```

It would work even if you just wrote this: 
```Python
mapped_key = sorted_keys[(index)]
```

# Solution 3

I just changed the Get method to post method in the submit route. And I changed the variable name from name to person-name, the way it was declared in the HTML script.
