# run-chrome-as-root
Run google chrome as another user when logged in as root

#### create a user called `chrome`

`# adduser chrome`


`google-chrome.sh`
```bash
#!/bin/bash

xhost +
su chrome <<'EOF'
/usr/bin/google-chrome-stable --incognito
EOF

```

```
# chmod +x ./google-chrome.sh
# ./google-chrome.sh
```
