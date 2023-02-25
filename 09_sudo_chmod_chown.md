##### sudo, chmod, chown

1. sudo: tài khoản phân quyền

* kí tự đầu tiên:

    - d: directory đầu tiên
    - -: file đầu tiên
    - l: shotcust đầu tiên
    - r: đọc
    - w: ghi
    - x: thực thi
    - -: không có quyền
    

* 3 kí tự tiếp
    - Owner

* 3 kí tự tiếp
    - Group


* 3 kí tự tiếp
    - Orther



- User : Cột 1
- Group: Cột 2
- Other: Còn lại



2. chmod: thiết lập chế độ phân quyền

- chmod u=rwx, g=rx, o=r __filename


3. chown: chuyển quyền cho tài khoản

- sudo chown root __filename

