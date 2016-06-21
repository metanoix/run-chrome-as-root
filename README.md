# run-chrom-as-root
Run google chrome as another user when logged in as root


```bash
#!/bin/bash

xhost +
su chrome <<'EOF'
/usr/bin/google-chrome-stable --incognito
EOF

```
