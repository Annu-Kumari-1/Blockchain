## Commands (IPFS)
## Install the IPFS through WSL: wget https://dist.ipfs.tech/kubo/v0.32.1/kubo_v0.32.1_linux-amd64.tar.gz 
 Or 
# wget https://github.com/ipfs/kubo/releases/download/v0.32.1/kubo_v0.32.1_linux-amd64.tar.gz
- ``` tar -xvzf kubo_v0.32.1_linux-amd64.tar.gz ```
- Kubo is a reference implementation of IPFS in Go: ``` cd kubo ```
``` ls
sudo bash install.sh
ipfs –version
ipfs init
ipfs daemon
On Browser: http://127.0.0.1:5001/webui
To run ipfs daemon in background: ipfs daemon > ipfs.log 2>&1 &
This is daemon ID: [1] 772
# Add file: echo "Hello, IPFS!" > ``` hello.txt
ipfs add hello.txt
ipfs cat <CID>
Add a directory: 
mkdir myfolder
echo "File 1 content" > myfolder/file1.txt
echo "File 2 content" > myfolder/file2.txt
ipfs add -r myfolder
ps aux | grep ipfs
kill <PID>
in Browser you can directly run this to see the IPFS: https://ipfs.io/ipfs/QmWd9cavD8UGZQcqYBVhZqs2Jure5W9cgxR7S6TC4StfZe
