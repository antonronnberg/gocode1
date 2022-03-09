# gocode1
Golang coding


Setup
---
Download Golang
https://go.dev/dl/

Run .msi installer - "go.1.17.8.windows-amd64.msi"

Select install location
C:\Program Files\Go
and step through install wizard

Check Windows Environment Variables ->
windows search -> sysdm.cpl -> Environment Variables
Select Edit for "Path" under User vaiables -> locate "C:\Program Files\Go\bin"

Next step add "GOPATH" to System variables
Locate where the path is pointed by checking in cmd -> go env
set GOPATH=[path showing here should be used as value for System variable]

Create symbolic junction to point GOPATH path to storage location on interest.
mklink /J "C:\Users\anton\go" "C:\Users\anton\OneDrive\Programming\go"

Now it should be possible to run
go mod init main
go build
and it will generate an executable file.

Note: prompt for install of packages have to get completed also.
---
