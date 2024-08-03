```ssh
TASK [Create hng user with sudo privileges] ************************************
fatal: [18.119.160.79]: FAILED! => {""msg"": ""Unable to encrypt nor hash, passlib must be installed. No module named 'passlib'. Unable to encrypt nor hash, passlib must be installed. No module named 'passlib'""}

TASK [Create hng user with sudo privileges] ************************************
fatal: [hng]: FAILED! => {""msg"": ""Unable to encrypt nor hash, passlib must be installed. No module named 'passlib'. Unable to encrypt nor hash, passlib must be installed. No module named 'passlib'""}

PLAY RECAP *********************************************************************
hng                        : ok=2    changed=1    unreachable=0    failed=1    skipped=0    rescued=0    ignored=0
