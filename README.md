py-4chan
========

Python Wrapper for 4chan API. Uses requests, respects if-modified-since headers on updating threads. Caches thread objects. Fun stuff.

### Sample Usage

``` python
import py4chan
b = py4chan.Board('b')
thread = b.getThread(423491034)

print thread

for file in thread.Files():
    print file
    
# In a while...
print "I fetched," thread.update(), "new replies."
```

API Documentation coming soon, but you can figure most of it out from the source. It's not rocket science.

# License

``` text
DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
                    Version 2, December 2004

 Copyright (C) 2004 Sam Hocevar <sam@hocevar.net>

 Everyone is permitted to copy and distribute verbatim or modified
 copies of this license document, and changing it is allowed as long
 as the name is changed.

            DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
   TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION

  0. You just DO WHAT THE FUCK YOU WANT TO.

```