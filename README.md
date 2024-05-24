# SQL-data-cleaning
Tải file CSV tên club_member_info
Tạo file text có tên club_member_info
Mở file mới tạo ra
Save as file mới tạo chọn All file, thêm đuôi .db vô tên file (club_member_info.db)
Chọn tab select database trên Dbeaver, chọn SQLite > next
Window xuất hiện, trong phần path nhấn open chọn file nguồn tên club_member_info.db
Tao DB

# import table customer
Import file csv

# tao bang clean (generate SQL ---> DDL)
  
  CREATE TABLE club_member_info_clean (
  	full_name VARCHAR(50),
  	age INTEGER,
  	martial_status VARCHAR(50),
  	email VARCHAR(50),
  	phone VARCHAR(50),
  	full_address VARCHAR(50),
  	job_title VARCHAR(50),
  	membership_date VARCHAR(50)
  );



# import value vao bang clean
INSERT INTO club_member_info_clean
    SELECT *
    FROM club_member_info;

# clean du lieu
