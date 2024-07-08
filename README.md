root@Switch-Lab:/home# command -v nvm
nvm
root@Switch-Lab:/home# nvm ls
            N/A
iojs -> N/A (default)
node -> stable (-> N/A) (default)
unstable -> N/A (default)
root@Switch-Lab:/home# nvm install --lts
Installing latest LTS version.
Downloading and installing node v20.15.0...
Downloading https://nodejs.org/dist/v20.15.0/node-v20.15.0-linux-x64.tar.xz...
######################################################################################################################################################################################################### 100.0%
Computing checksum with sha256sum
Checksums matched!
Now using node v20.15.0 (npm v10.7.0)
Creating default alias: default -> lts/* (-> v20.15.0)
root@Switch-Lab:/home# nvm ls
->     v20.15.0
default -> lts/* (-> v20.15.0)
iojs -> N/A (default)
unstable -> N/A (default)
node -> stable (-> v20.15.0) (default)
stable -> 20.15 (-> v20.15.0) (default)
lts/* -> lts/iron (-> v20.15.0)
lts/argon -> v4.9.1 (-> N/A)
lts/boron -> v6.17.1 (-> N/A)
lts/carbon -> v8.17.0 (-> N/A)
lts/dubnium -> v10.24.1 (-> N/A)
lts/erbium -> v12.22.12 (-> N/A)
lts/fermium -> v14.21.3 (-> N/A)
lts/gallium -> v16.20.2 (-> N/A)
lts/hydrogen -> v18.20.3 (-> N/A)
lts/iron -> v20.15.0
root@Switch-Lab:/home# node --version
v20.15.0
root@Switch-Lab:/home# npm --version
10.7.0
root@Switch-Lab:/home# cd react_app/
root@Switch-Lab:/home/react_app# nvm use --lts
Now using node v20.15.0 (npm v10.7.0)
root@Switch-Lab:/home/react_app# npm create vite@latest my-react-app -- --template react
Need to install the following packages:
create-vite@5.3.0
Ok to proceed? (y) y