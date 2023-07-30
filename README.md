# 3007anhNhat
3007anhNhat
Đầu tiên sẽ là làm vidu ngày hôm nay
Ví dụ: tìm ra top 5 sv có điểm cao nhất trong clb có nhiều người tham gia nhất
**B1: tạo tên bảng** 
CREATE DATABASE student;
**B2: tạo cơ sở dữ liệu trong bảng với các cột là "id", "name", "score" và "clb"**
CREATE TABLE students (
    idstudent INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(50) NOT NULL,
    score INT,
    clb VARCHAR(50)
);
**B3: thêm dữ liệu**
INSERT INTO students (id,name, score, clb) VALUES
1	Alice	85	Math Club
2	Bob	90	Science Club
3	Charlie	78	Chess Club
4	David	92	Art Club
5	Emma	88	Music Club
6	Frank	79	Debate Club
7	Grace	91	Drama Club
8	Henry	82	Football Club
9	Isabella	95	Science Club
10	Jack	87	Chess Club
11	Kate	84	Math Club
12	Liam	89	Music Club
13	Mia	76	Debate Club
14	Noah	93	Art Club
15	Olivia	81	Football Club
16	Oscar	90	Chess Club
17	Sophia	85	Math Club
18	Thomas	87	Science Club
19	William	88	Music Club
20	Zoe	79	Drama Club
21	Alice	85	Math Club
22	Bob	90	Science Club
23	Charlie	78	Chess Club
24	David	92	Art Club
25	Emma	88	Music Club
26	Frank	79	Debate Club
27	Grace	91	Drama Club
28	Henry	82	Football Club
29	Isabella	95	Science Club
30	Jack	87	Chess Club
31	Kate	84	Math Club
32	Liam	89	Music Club
33	Mia	76	Debate Club
34	Noah	93	Art Club
35	Olivia	81	Football Club
36	Oscar	90	Chess Club
37	Sophia	85	Math Club
38	Thomas	87	Science Club
39	William1	78	Music Club
40	William2	58	Music Club
41	William3	48	Music Club
42	William4	28	Music Club
43	Zoe	79	Drama Club

**B4: Tìm ra clb có nhiều người tham gia nhất**
SELECT clb, COUNT(*) AS member_count
FROM student
GROUP BY clb
ORDER BY member_count DESC
LIMIT 1;
====> Music Club	15
**B5: Tìm ra 5 người có điểm số cao nhất trong 15 người đó**
SELECT *
FROM student
WHERE clb = 'Music Club'
ORDER BY score DESC
LIMIT 5;
====> ![image](https://github.com/vietdtds/3007anhNhat/assets/104219452/3c40aca2-83aa-4d03-91a5-3709938b1b31)
**Kết thúc!**

Hôm nay 30/07
1. Cần xem lại và code thử các hàm của Java collection
So sánh độ phức tạp của phương pháp
Độ phức tạp của hash table trong việc tìm kiếm xóa và là O(log(n)) vì đã được sắp xếp thứ tự key theo tăng dân 
Dưới của hashmap là hashtable(lưu trữ bằng phương thức hashtable) vì vậy độ phức tạp của hashmap , linkedhashmap, tree map cx giống như hash table về tìm kiếm xóa 
của linked khi thêm mới là O(1) 
Đặc biệt là tìm hiểu thì nên tìm hiểu lý thuyết bằng tiếng anh, thực hành nhiều hơn
2. Về SQL thì hnay tìm hiểu chính về cấu trúc và làm 1 ví dụ cụ thể như ở trên
scheme -> database -> table -> column
Các bài toán thì cần chia nhỏ để làm (như là chia để trị)
Lamf nhiều bài toán về SQL hơn, đang còn yếu
Đặc biệt là phần SQL keywords xem đã hiểu được bao nhiêu và cần học thêm những gì
BTVN: Tìm hiểu CONNECTION Pool, cũng như chủ động học báo lại kết quả cho anh và mọi người xem
   Chỉ anh Đức phần github để anh làm pp review cho mọi người

    
