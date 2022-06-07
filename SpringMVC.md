# SPRING MVC

## Maven
1. Định nghĩa : Maven là công dung de quan ly project Spring MVC
2. Maven duoc phat trien boi Apache
3. Maven giup download va quan ly cac thu vien (dependencies) cua project
4. Maven quan ly cac ban build, thong tin Team, phien ban
5. Chu ky song cua Maven:
  + POM.xml : file cau hinh cua du an, file pom.xml la noi khai bao cac dependency, version cua du an, ten du an ...
  + Build: Tep lenh maven
  + Dependencies: thu vien can dung trong project
  + Repository: Noi luu tru thu vien
  + Plugins: libs can chay project
  + Profiles: build khac nhau

## Cách hoạt động của SPRING MVC
1. request gui den Dispatcher Servlet
2. Dispatcher Servlet kiem tra request, dieu huong request den Controller thong qua Handler Mapping
3. Controller tao va model va goi view => Tra ve lai Dispatcher Servlet
4. Dispatcher Servlet tim viewName
5. View ket hop voi model tra ve cho nguoi dung duoi dang respone

- IoC container : dung de khoi tao doi tuong tu 1 class, cau hinh, quan ly va dieu phoi cac doi tuong bean trong chuong trinh
- Bean : la cac doi tuong duoc khoi tao tu 1 class, Ton tai trong khung lam viec cua request, session, appication context
  + Singleton: 1 doi tuong duy nhat trong IoC. hay dung
  + Prototype: 1 doi tuong moi duoc tao ra khi goi den bean. it dung
- 


