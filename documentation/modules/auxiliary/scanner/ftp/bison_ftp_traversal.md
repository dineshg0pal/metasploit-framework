## Description

This module exploits a directory traversal vulnerability in BisonWare BisonFTP Server version 3.5.

An attacker can retrieve arbitrary files from the server by sending a specially crafted RETR command containing traversal sequences such as `..//.`.

This allows access to sensitive files on the system (e.g., `boot.ini`).

## Module Name

auxiliary/scanner/ftp/bison_ftp_traversal

## Author

- Jay Turla
- James Fitts
- Brad Wolfe

Documentation added by: YOUR_NAME

## References

- CVE-2015-7602
- https://www.exploit-db.com/exploits/38341

## Platform

Windows

## Targets

BisonWare BisonFTP Server 3.5

## Options

- **RHOSTS**: Target host(s)
- **RPORT**: Target FTP port (default: 21)
- **DEPTH**: Traversal depth to reach root directory (default: 32)
- **PATH**: File path to retrieve (default: boot.ini)

## Usage

1. Start Metasploit:
   ## Description

This module exploits a directory traversal vulnerability in BisonWare BisonFTP Server version 3.5.

An attacker can retrieve arbitrary files from the server by sending a specially crafted RETR command containing traversal sequences such as `..//.`.

This allows access to sensitive files on the system (e.g., `boot.ini`).

## Module Name

auxiliary/scanner/ftp/bison_ftp_traversal

## Author

- Jay Turla
- James Fitts
- Brad Wolfe

Documentation added by: YOUR_NAME

## References

- CVE-2015-7602
- https://www.exploit-db.com/exploits/38341

## Platform

Windows

## Targets

BisonWare BisonFTP Server 3.5

## Options

- **RHOSTS**: Target host(s)
- **RPORT**: Target FTP port (default: 21)
- **DEPTH**: Traversal depth to reach root directory (default: 32)
- **PATH**: File path to retrieve (default: boot.ini)

## Usage

1. Start Metasploit:
   ## Description

This module exploits a directory traversal vulnerability in BisonWare BisonFTP Server version 3.5.

An attacker can retrieve arbitrary files from the server by sending a specially crafted RETR command containing traversal sequences such as `..//.`.

This allows access to sensitive files on the system (e.g., `boot.ini`).

## Module Name

auxiliary/scanner/ftp/bison_ftp_traversal

## Author

- Jay Turla
- James Fitts
- Brad Wolfe

Documentation added by: Dinesh Gopal

## References

- CVE-2015-7602
- https://www.exploit-db.com/exploits/38341

## Platform

Windows

## Targets

BisonWare BisonFTP Server 3.5

## Options

- **RHOSTS**: Target host(s)
- **RPORT**: Target FTP port (default: 21)
- **DEPTH**: Traversal depth to reach root directory (default: 32)
- **PATH**: File path to retrieve (default: boot.ini)

## Usage

1. Start Metasploit:
   
msfconsole
   
2. Load the module:

use auxiliary/scanner/ftp/bison_ftp_traversal

3. Set target:

set RHOSTS <target_ip>

4. (Optional) Set file path:

set PATH boot.ini

5. Run:

run

## Example Output

[+] Stored boot.ini to /root/.msf4/loot/...


## Notes

- The module requires valid FTP connectivity.
- Successful exploitation depends on server configuration.
- The retrieved file is stored as loot in Metasploit.
