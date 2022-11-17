# **Tổng quan Java cơ bản**
- ### **Đoạn code cơ bản** <br>
File `Main.java`:
```java
    public class Main {
        public static void main(String[] args){
            // Đoạn code sẽ được bắt đầu ở đây
        }
    }
```
- Note: <b> Vì tên class phải khớp với tên file nên khi đặt tên file hãy viết hoa chữ cái đầu để tránh trường hợp trùng với từ khóa riêng của Java.</b>

- ## **Output**
    + `System.out.println(" ")`
- ## **Comment**
    + 1 dòng : `//`
    + Nhiều dòng: `/* */` 
- ## **Biến**
    + Biến bình thường: ( Giống C++ )
    + Biến hằng:
        Chỉ cần thêm từ khóa **`final`** vào trước cú pháp khai báo biến.
      VD:
      ```java
        final (kiểu dữ liệu)(tên biến);
        // VD:
        // final String newString;
      ```
    + Ép kiểu: ( Giống C++ );

- ## **Toán tử**
    + ( Giống C++ )
- ## **Xử lí chuỗi**
    + Cách sử dụng: ( Giống C++ )
    + Hàm thường dùng:
        + **`length()`** : Kiểm tra độ dài của chuỗi
        + **`toUpperCase()`** : Ép chuỗi sang dạng viết hoa.
        + **`toLowerCase()`** : Ép chuỗi sang dạng viết thường.
        + **`indexOf()`** : Chỉ ra vị trí bắt đầu xuất hiện lần đầu tiên của chuỗi cần kiểm tra.
        + **`concat()`** : Ghép chuỗi.
    + Cách ghép kí tự đặc biệt vào trong chuỗi:
        + Sử dụng **`\`** ở trước mỗi kí tự đặc biệt.
- ### **Math**
    + Hàm sẵn có:
        + **`min(a, b)`** : GTNN giữa `a` và `b`
        + **`max(a, b)`** : GTLN giữa `a` và `b`
        + **`abs(x)`** : GT tuyệt đối dạng dương (+) của `x`
        + **`sqrt(x)`** : Căn bậc 2 của `x`
        + **`random()`** : Sẽ trả ra một số thập phân ngẫu nhiên từ `0.0` đến `1.0` theo mặc định.<br>
        Hoặc nếu muốn chọn điểm bắt đầu và điểm kết thúc thì:<br>
        **`(int)(Math.random() * số lượng số tự nhiên cần thêm);`**
- ### **If-else**
    + ( Giống C++ )
- ### **Switch**
    + ( Giống C++ )
- ### **Vòng lặp**
    + ( Giống C++ )
- ### **Mảng**
    + Khai báo: <br>
        + Dạng 1 chiều: `(Kiểu dữ liệu)[] (tên mảng)`
        + Dạng đa chiều: `(Kiểu dữ liệu)[][] (tên mảng)`
    + Có thể truy cập vào phần tử của mảng theo chỉ số (index). Phần tử đầu tiên là 0.
- ### **Phương thức**
    + Khai báo: <br>
    ```java
        public void (tên hàm)(){
            // Code sẽ được triển khai trong này
        }
    ```
    hoặc là:
    ```java
        public (tên hàm)() {
            // Code sẽ được triển khai trong này
        }
    ```
    + Overload: ``(Có thể hiểu là "sử dụng lại")``<br>
    Tức là phương thức có thể cùng tên và thực hiện cùng một công việc trong khi kiểu dữ liệu và biến số của hàm có thể khác.
    + Scope: ``(Có thể hiểu là "khu vực")``<br>
    Tóm tắt nhanh là: <br>
        <b>
        ```
        Biến được khai báo ở khu vực nào thì chỉ khu vực ở đó mới có thể sử dụng biến đó, còn nếu biến được khai báo trong một block thì chỉ trong block đó mới có thể dùng biến đó.
        ```
        </b>