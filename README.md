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
