---
layout: single
title: "How to set Oracle jdbc url"
---

# oracle jdbc url 설정하는 방법

oracle DB를 이용하여 데이터베이스를 사용할 때 <br/>

jdbc의 url은 <br/>

jdbc:oracle:thin:@hostname:port:SID <br/>

와 같은 순으로 설정해야 한다. <br/>

hostname에는 listener.ora, tnsnames.ora에 적혀있는 hostname(IP 혹은 컴퓨터이름)을 적어주면 된다. <br/>

## 경로 <br/>
<code>oraclexe\app\oracle\product\11.2.0\server\network\ADMIN</code>
