# CTDL-GT_Tail_Recursion_2.cpp
Tail Recursion
Nguồn tham khảo : https://freetuts.net/de-quy-duoi-tail-recursion-2951.html

Ví dụ : hàm đệ quy UCLN() để hiểu về đệ quy đuôi rõ  :

+ code : 
int UCLN(int m, int n){
  int r;
  if(m<n) return UCLN(n,m);
  r = m % n;
  if(r == 0) return n;
  else return UCLN(n,r);
}

+ Hình ảnh minh họa :

  - lấy tham số truyền vào cho hàm UCLN() là m = 25 và n = 5 : 
  
![co-che-de-quy-duoi](https://user-images.githubusercontent.com/129465517/230533750-2a15f7b0-71e7-4d3d-b5a5-257bd50ddde6.png)
