# Keylogger - Nâng cao

## Documentation
### Setup
> 

Truy cập vào folder chứa code đã clone
> pip install -r requirements.txt

### Run
> python logserver\server.py 
_#Dùng để chạy server nhận dữ liệu_

> python clientapp\keylogger.py
_#Dùng để chạy keylogger_

> python owner\handle_logs.py
_#Dùng để logs người dùng nhập từ bàn phím trực tiếp_

### Logs
Truy cập vào api từ server được hiển thị ở debug message khi chạy `server.py`

Ví dụ server: `http://localhost:5000`

API để lấy logs: http://localhost:5000/api/logs

API để lấy raw logs (logs chưa được xử lí): http://localhost:5000/api/rawlogs

API để clear logs: http://localhost:5000/api/flush_logs

### Executable
> pyinstaller clientapp\keylogger.py
_#pip install pyinstaller_

### Host
Bạn có thể dùng port forwarding để người dùng keylogger có thể connect vào server hoặc dùng chung một mạng (LAN). Bạn có thể dùng bên thứ ba để host code.
