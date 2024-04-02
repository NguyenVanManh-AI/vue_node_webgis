# vue_node_webgis
0. Run fe + be : npm i 
1. Open pgAdmin4 to create database : Ex : gkwebgis
2. Open : C:\Users\ADMIN\Downloads\vue_node_webgis\be\.env 
    + DATABASE_URL="postgresql://postgres:hivanmanh@localhost:5432/gkwebgis"
        + 'hivanmanh' is password 
        + 'gkwebgis' is name database 
3. Remove folder : C:\Users\ADMIN\Downloads\vue_node_webgis\be\prisma\migrations
4. Run be : npx prisma migrate dev --name init
5. Run be : npm start 
6. Run fe : npm run dev 
7. Go to : http://localhost:9000/login to Register account 
    + email : nguyenvanmanh2001it1@gmail.com 
    + pw : nguyenvanmanh2001it1
    + confirm pw : nguyenvanmanh2001it1
8. Go to Database : gkwebgis to Edit Role account from USER to ADMIN 
9. Go to file : C:\Program Files\GeoServer\webapps\geoserver\WEB-INF\web.xml => Edit same file vue_node_webgis/web.xml (copy file này dán vào file WEB-INF\web.xml)
    + Search dưới task bar : Stop GeoServer => click 
    + Search dưới task bar : Start GeoServer => click 
10. Go : http://localhost:9000/projection-management => Thêm trục chiếu : 'EPSG:4326'
11. Go : http://localhost:9000/location-management => Thêm điểm , Ex 
    + Tên : 120 Nguyen Luong Bang 
    + Kinh độ : 108 
    + Vĩ độ : 16 
    + Workspace : MapDaNang (chọn đại một workspace là được)(không có thì tạo thêm)
12. Tại điểm đó : Sổ xuống : Các lớp bản đồ => Url là link dạng Json 
    + Go to : http://localhost:8080/geoserver/web/wicket/bookmarkable/org.geoserver.web.demo.MapPreviewPage?1&filter=false => Đặt tên ví dụ : Test2
    + Search : Ex : VNM => All Formats chọn GeoJSON => Open ra một tab mới => copy link đó cho vào 
12.a Quay lại bản đồ : http://localhost:9000/map => chọn địa điểm => thanh bên trái => 'ĐỊA ĐIỂM' => chọn Test2 (lớp mình đã thêm vào ở trước)

