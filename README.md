# Sandbox

inner clickable link with fr accent:
[title with é](#title-with-é)


a

a

a

a

a

a

a

a

a

a

a

a

a

a

a

a

a

a

a

a

a

a

a


# title with é

a

a

a

a


# and if there is no emtpy line

b
c
d



# with list

- b
- c
- d

# with list and title

## better
- b
## better
- c
- d

# with list and *text*

**better**
- b
**better**
- c
- d

# with list and *text*
  b
  c
  d
  
# with list and *text*

  **better**
- b

  **better**
- c
- d

# with list and *text*
 **better**
- b
 **better**
- c
- d

  __a2dissite__
* _mod_ - The conf file in sites-enabled to be moved to sites-available
* _add_ - `-mod` will name a path to a file to be moved to sites-available
* _norestart_ - Don't restart the web server on completion


# and if there is no emtpy line

  - **A**
  - b
  - **A**
  - c
  - d



## Usage  

  __a2enmod [[-m[od]] \<String\> [[-s[earch]] \<String\>] [-r[eplace]] [-c[opy]] [-n[orestart]]]__
* _mod_ - The module to enable or add
* _search_ - The path to the module.
* _replace_ - Replace the path in the LoadModule line for this module with the file path passed to _search_.
* _copy_ - A new module will be added and the file will be copied to the default modules directory.
* _norestart_ - Don't restart the web server on completion

Locates the specified module and uncomments its LoadModule line to enable it. A new module will be added if a path to a valid file is passed to `-search`. The new LoadModule line will be appended to the long list of enabled and disabled lines that usually comes with Apache. `-copy` will make a copy in the default modules folder. If `-mod` names a newly added module, it must be the same name specified by the module file. If referring to a module already specifed in the conf, it may be named by either the part before `_module`, the full module name, filename, or basename (filename without extension).
	
  __a2dismod [[-m[od]] \<String\> [-n[orestart]]]__
* _mod_ - The module to disable
* _norestart_ - Don't restart the web server on completion

Adds a comment marker to the LoadModule line of the specified module to disable it.


# and if there is no emtpy line

  **A**
- b
- c

  **B**
- d


	a2ensite
Show information about enabled and disabled sites.

	a2ensite mysite
Enables the site defined in the file ServerRoot\conf\sites-available\mysite.conf.

	a2ensite C:\my\folder\mysite.conf -add
Move the Virtual host configuration defined in C:\my\folder\mysite.conf to ServerRoot\conf\sites-enabled.

	a2ensite C:\my\folder\mysite.conf -c
Copy mysite.conf from the specified folder into sites-enabled, then enable it.

	a2ensite mysite –norestart
Move ServerRoot\conf\sites-available\mysite.conf to ServerRoot\conf\sites-enabled, but don’t restart the web server.

	a2dissite mysite
Disable ServerRoot\conf\sites-enabled\mysite.conf by moving it to sites-available and restarting the web server.



**change password**

passwd (change password for debian user)
sudo passwd root (change root password)

**update system**
sudo apt update
