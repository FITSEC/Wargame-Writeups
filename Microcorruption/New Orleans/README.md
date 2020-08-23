New Orleans
=====

> First level of Microcorruption

## Solution
First thing I did was set a breakpoint on main and continue execution of the program. I noticed a create_password function being called and stepped into this function. 

![](img/flag.png)

It looked like ascii range bytes were being loaded into r15, so I annotated these bytes as I had a hunch this was the password being created. I went ahead and continued execution. I was prompted for the password and checked the box for inputing hex encoded input: "3c7e4267384c44" and clicked send. I continued e
xecution and the door unlocked!


> 3c7e4267384c44
