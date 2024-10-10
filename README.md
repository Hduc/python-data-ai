### Bước 1 cài đặt scoop để
```
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
Invoke-RestMethod -Uri https://get.scoop.sh | Invoke-Expression
```
### Bước 2 Cài đặt pipx
```
scoop install pipx
pipx ensurepath
```
### Bước 3 Cài đặt cookiecutter-data-science để tạo template  python
```
pipx install cookiecutter-data-science
```
### Bước 4 tạo template thư mục bằng lệnh
```
$env:path = $env:path + ";C:\Users\duc.nguyen\.local\bin"

ccds
```
