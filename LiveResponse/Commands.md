

# General

# Identity

## User information


## Listing all users
```execfg powershell net users```

## Listing local admins
```execfg powershell net localgroup administrators```

## Listing local groups
```execfg powershell net localgroup```

## Listing Kerberos tickets
```execfg powershell klist sessions```

##

# System

## Get computer information
```execfg powershell get-computerinfo```
```execfg powershell systeminfo```
```execfg powershell wmic computersystem list full```

## Drives connected to the computer
```drives```
```execfg powershell fsutil fsinfo drives```

## Installed updates
```execfg powershell wmic qfe```

## Installed softwares
```execfg powershell wmic product get name,version```
```execfg powershell get-package```

# Network

## Getting network configuration
```execfg powershell ipconfig /all```

## Listing active connections
```execfg netstat -anob```

# Process 

# File

## Listing shares
```execfg powershell net share```

## Listing all files on computer
```
execfg powershell tree c:\ /F > files.txt
get files.txt
execfg powershell rm files.txt
```

## Download a file
```get <filename>```

## Get hash of file
```execfg powershell get-filehash <filename>```

## Search for string pattern recursively
```execfg findstr /s /i "<pattern>" *```

## Print content of file in live console
```execfg powershell gc <filename>```

