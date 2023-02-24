# cat, echo, tail, grep

1. cat: xem nội dung file và ghép nội dung của file vào một file duy nhất

- cat __namefile => in nội dung file
- cat __file1 __file2 => ghép các file vào với nhau
- cat __file1 __file2 > __file3 => gom file 1 và file 2 vào file 3

2. echo: in nội dung ra màn hình

- echo "Nguyễn Duy Khánh"
- echo "<h1> Nguyễn Duy Khánh </h1>" > __filename => lưu nội dung vào file name ghi nhiều lần thì ghi đè
- echo "<h1> Nguyễn Duy Khánh </h1>" >> __filename => không ghi đè vào file in ra nhiều dòng


3. tail: kiểm tra nội dung mới nhất của file

- p*100{item $} => enter
- tail -n <số dòng> __filename
- tail -f __filename: folow file update trực tiếp file


4. grep: tìm kiếm từ xuất hiện stout

- cat __filename | grep __từ cần tìm
- cat __filename __filename | grep __từ cần tìm