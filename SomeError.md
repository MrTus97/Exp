#vscode
1. Khi run terminal ở visual studio code mà không thể active được env như bên dưới
Lỗi:
```shell
$ .\env\Scripts\activate
.\env\Scripts\activate : File <path>\env\Scripts\Activate.ps1 cannot be loaded because running 
scripts is disabled on this system. For more information, see about_Execution_Policies at 
https:/go.microsoft.com/fwlink/?LinkID=135170.
```
Sửa bằng cách
```shell script
$ set-ExecutionPolicy -Scope Process ByPass
```
