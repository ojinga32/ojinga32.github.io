---
layout: single
title: "The network adapter could not establish the connection error and solution"
---

# The network adapter could not establish the connection 원인, 해결
**oracle과 sql developer를 다운받고 커넥션을 해주면 이렇게 에러가 생겼다.**
![ora5](https://github.com/ojinga32/ojinga32.github.io/assets/133554766/c1d05b42-43fc-4a1b-ab23-b9cfaefc6467)

<br/><br/>

## 원인
여러가지의 원인이 있었는데 먼저 나의 원인은 <br/>
<code>C:\app\user\product\21c\homes\OraDB21Home1\network\admin</code>
이 경로에 listener.ora 파일과 tnsnames.ora 파일의 설정에 에러가 있었다<br/>

![ora7](https://github.com/ojinga32/ojinga32.github.io/assets/133554766/caf0a525-822f-49f0-aff7-d57c5ffb6d94)
![ora8](https://github.com/ojinga32/ojinga32.github.io/assets/133554766/3ec5a817-0a3e-490a-8601-435e12ae639f)

그림에 host가 나의 잘못된 ip주소로 바뀌어 있었다.

## 해결 방법
host에 나의 옳바른 ip를 써줘도 괜찮지만 나의 pc 이름을 적어줘도 괜찮다

**내 pc이름 확인하는 법**
1. 내  PC 우클릭
2. 속성
3. 장치 이름이 나의 PC이름이다

![ora6](https://github.com/ojinga32/ojinga32.github.io/assets/133554766/216b5a4f-a195-48b4-99bf-c65f7f5ecf58)

그림과 같이 host의 이름을 변경 해주었다. 그 결과
![ora3](https://github.com/ojinga32/ojinga32.github.io/assets/133554766/b5bb8852-2fc0-40f1-97da-df82cccd4f2e)
모든 리스너가 정상적으로 작동되었고

![ora4](https://github.com/ojinga32/ojinga32.github.io/assets/133554766/99937815-b5fe-44f9-903e-44739858d4d2)
커넥션도 성공





