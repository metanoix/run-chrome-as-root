# run-chrom-as-root
Run google chrome as another user when logged in as root


`google-chrome.sh`
```bash
#!/bin/bash

xhost +
su chrome <<'EOF'
/usr/bin/google-chrome-stable --incognito
EOF

```

`
# chmod +x ./google-chrome.sh`
# ./google-chrome.sh
`
