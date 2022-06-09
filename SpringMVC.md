# SPRING MVC : la 1 phan cua spring framework

- Spring mvc ho tro Inversion of controll va Dependency Injection
- Spring mvc su dung DispatcherServlet de don request de xu ly
- cong cu xu ly dua vao @Controller va @RequestMapping annotations

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
## Y nghia cac annotations
- @Controller: chi dinh class nao do lam trung tam dieu khien, xu ly request va tra ve response
- @RequestMapping: khai bao o tren method, chi dinh phuong thuc HTTP nao se duoc ap dung cho method va URL cua request
    + @GetMapping: 1 cach ngan gon hon khi dung phuong thuc HTTP GET
    + @PostMapping:  tuong tu
- Cac property trong @GetMappng, @PostMapping : path="", consumes="", produces="" ..., tim hieu them
- @RequestBody: la gi???

## ViewResolver and View : 2 interface
- Day la 2 interface quan trong duoc Spring su dung de xu ly views
- ViewResolver cung cap mapping giua view names va acutal views
- View : ????
- Resolving Views thuong tra ve String, View hoac ModelAndView instance;
- 


