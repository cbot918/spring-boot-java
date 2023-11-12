# Spring Boot Getting Started

0. 環境設定一下

   0.1 裝一下 maven: java 用的套件管理( 對標 npm )

   0.2 jdk jre 需要 17 ( 裝一下 jdk/jre17, 然後 JAVA_HOME 設定過去, 可以參考一下網路教學)

1. vscode Ctrl+Shift+P 開啟 panel > 輸入 java > 點 help center > 點 create project

2. 選 Spring Boot > 選 Maven Project > 選 3.1.5 > 選 Java > com.java 按 enter > 這邊取個專案名稱 > 選 Jar > 選 17 > 選 select 0 > 然後視窗指定專案儲存位置

3. maven 安裝依賴( 依賴在 pom.xml 裡面看 ): `mvn clean install`

4. pom.xml 裡面改個東西 [搜尋下] spring-boot-starter 改成 spring-boot-starter-web (不然不會監聽)

5. run 專案: `mvn spring-boot:run` (預設 port 是 8080, 所以可能先確保系統內 8080 空著, 或是在 application.properties 裡面加個 server.port=8081 設定)

6. 瀏覽器去 localhost:8080 看, 可能頁面不存在, 但 terminal 裡面應該會有 request log 進來, 就代表專案啟動, Spring Boot Hello World 成功！
