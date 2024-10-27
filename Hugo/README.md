# Hugo 👈🏻
# Static website development

---
---
---

# Azure servers (Microsoft)

https://portal.azure.com/

anumit@hotmail.com

SSH login imformation -

20.78.10.127

firstuser

Password1!Password2!

Networking - Add ports rule to allow all incoming and ourgoing traffic


## Linux Terminal Text editor

nano

## Install Node.js

sudo apt update

sudo apt install nodejs

node -v

## Install NPM: npm (Node Package Manager)

sudo apt install npm


--- 
---
---

# Hugo Quick start
https://gohugo.io/getting-started/quick-start/

hugo new site quickstart

cd quickstart

git init

git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke.git themes/ananke

echo "theme = 'ananke'" >> hugo.toml

hugo server


hugo server --bind 0.0.0.0

http://20.78.10.127:1313

---

# Hugo - Coding 

/home/firstuser/mycode/websites/hugo/website1

cd /home/firstuser/mycode/websites/hugo/website1

Alias

alias ll="ls -alF"


## build files in public folder 
hugo

## zip in public folder 
zip -r foo.zip .

/home/firstuser/mycode/websites/hugo/website1/quickstart/public

cd /home/firstuser/mycode/websites/hugo/website1/quickstart/public

## Downlaod zip files using FTPManager

cd /home/firstuser/mycode/websites/hugo/website1/

## upload the zip file to public ftp server

cd /home/firstuser/mycode/websites/hugo/website1/quickstart/public

curl -T foo.zip ftp://ftp.dlptest.com --user dlpuser:rNrKYTX9g7z3RgJRmxWuGHbeu

## download files from the same public ftp server to local drive

use iPad software called ftp lite

FTP URL: ftp.dlptest.com or ftp://ftp.dlptest.com/

FTP User: dlpuser

Password: rNrKYTX9g7z3RgJRmxWuGHbeu


## upload files to cloudflare pages
open cloudflare dashboard

https://dash.cloudflare.com

Go to section titled "Workers and Pages"

upload the foo.zip file

Open your website at - 

https://test-4be.pages.dev

---
---
---
# Upload large files from local to Azure VM

## 1. upload to google drive
## 2. ftp the file from google drive to Azure VM

upload to google drive and get shareable link

get fioe identifier from the url 

Inside Azure VM
use the following shell script to downlaon the large zip file - 
```
#!/bin/bash
fileid="FILEIDENTIFIER"
filename="FILENAME"
curl -c ./cookie -s -L "https://drive.google.com/uc?export=download&id=${fileid}" > /dev/null
curl -Lb ./cookie "https://drive.google.com/uc?export=download&confirm=`awk '/download/ {print $NF}' ./cookie`&id=${fileid}" -o ${filename}

```

---
---
---

# Responsive Website Test

https://usepastel.com/responsive-website-test







































































