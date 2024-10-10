### Bước 1 cài đặt scoop để

```
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
Invoke-RestMethod -Uri https://get.scoop.sh | Invoke-Expression
```
### Bước 2 Cài đặt pipx

```
scoop install pipx
pipx ensurepath

scoop install git 
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

### Bước 5 Cài đặt các gói tách biệt với môi trường bên ngoài
> chảy terminal ở bash (không phải powershell)
`python -m venv .venv`
`source .venv/Scripts/activate`
### Bước 6 Cài đặt các gói liên quan
`pip install -r requirements.txt`

### Bước 7 chạy
`streamlit run Chart_With_Your_Data.py`