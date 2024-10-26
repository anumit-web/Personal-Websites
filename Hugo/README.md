# Hugo 👈🏻

---

# Azure servers (Microsoft)

https://portal.azure.com/

anumit@hotmail.com

SSH login imformation -

20.78.10.127

firstuser

Password1!Password2!

Networking - Add ports rule to allow all incoming and ourgoing traffic


## Text editor

nano

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








































































