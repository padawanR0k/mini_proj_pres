---
theme: gaia
size: 16:10
_class: lead
paginate: true
slide-transition: true
# backgroundColor: #0093E9
# backgroundImage: linear-gradient(160deg, #0093E9 0%, #80D0C7 100%);
backgroundImage: url('https://64.media.tumblr.com/ee843139aadcb41fa338d57431c5ee9c/tumblr_oiwyu3PV5S1tf8vylo1_1280.png')
marp: true
---

![bg left:40% 70%](https://user-images.githubusercontent.com/819186/51553744-4130b580-1e7c-11e9-889e-486937b69475.png)

# **Slack bot**

파이썬을 사용한 슬랙봇 <br/>
	조원: 이유록


---
# 내가 필요한 걸 만들자

- ~~당근마켓 알림 서비스 중고나라, 번개장터 버전~~
	- 생각할게 너무 많아서 취소
- ~~일정시간마다 알림을 주는 스트레칭 알리미~~
	- 응용프로그램으로 만드려고 하니, 처음 생각보다 어려워서 취소
- 챗봇
	- 자료도 많고, 혼자 할만 할거같다.
	- 다른사람에게 공유하기 편하며 접근성이 편하다.
---
# 어떤 플랫폼을 고를까

![bg left:30% 50%](https://www.flaticon.com/svg/static/icons/svg/2111/2111466.svg)
![bg right:30% 50%](https://user-images.githubusercontent.com/819186/51553744-4130b580-1e7c-11e9-889e-486937b69475.png)
###### 카톡
- 관련 자료가 비교적 적음. 보낼 수 있는 메세지 형태가 슬랙보다 다양하지 않음
- 전화번호가 하나 더 필요..

###### 슬랙
- 관련 자료가 비교적 많음. 보낼 수 있는 메세지 형태가 카톡보다 훨씬 다양함
- 이메일만 있으면됨

---
# 슬랙 워크스페이스
- https://playdatastubot.slack.com/archives/C01EY4N7CRX
	- [일반] 채널

---
# 기능 1 - 특정 지역의 날씨정보 조회
![bg left:45% w:540](./feature_weather.webp)
- 명령어
	- `@playdata_stu_bot /날씨 서초구`
- 입력한 지역의 현재 날씨를 알려줍니다.


---
# 기능 2 - 개발 블로그 포스트 조회
![bg left:45% w:540](./feature_blog_post.webp)
- 명령어
	- `@playdata_stu_bot /블로그`
- 최근에 올라온 개발 관련 블로그 글들의 간단한 내용과와 링크를 알려줍니다.

---
# 기능 3 - 결석가능일 조회
![bg left:43% w:540](./feature_absent.webp)
- 명령어
	- `cnt`: 이번달 결석한 횟수
	- `@playdata_stu_bot /결석 cnt`
- 이번달 소정훈련일수와 이번달 결석한 횟수에 비례해서 재적위험까지 얼마나 남았는지 알려줌

---
# 기능 4 - 기능 확인
![bg left:43% w:540](./feature_help.webp)
- 명령어
	- `@playdata_stu_bot /help`
- 현재 봇에 등록된 기능들에 대한 설명서를 조회한다.

---
<!-- _class: follow -->
# 기능 5 - 퇴근처리 알림

![bg left:45% w:500](./feature_alram.png)
- 슬랙봇이 매일 오후 6시에 알림을 보내준다.
- ~~QR코드 이미지를 보내려고 했지만, 학원에서 금지하는 행위라 취소~~

---
# 기능 6 - 목 스트레칭 알림
![bg left:43% w:500](./feature_stretch.png)
- 9~17시 각 1시간 마다 스트레칭을 하라는 알람을 보내준다. `N시 50분`

---
# 기능 6_1 - 목 스트레칭 하기
![bg left:45% w:550](./feature_stretch_fron.png)
- google의 [teachable machine](https://teachablemachine.withgoogle.com/)을 활용한 신체 자세 감지
- [직접해보기](https://padawanr0k.github.io/tm_stretch_pos/)

---
# 사용 스택
- 서버 프레임워크
	- flask (python)
- 프론트
	- react (js)
- 배포 플랫폼
	- [heroku](https://www.heroku.com/)(서버), [github pages](https://pages.github.com/)(프론트)
---
# 느낀점
- 장점
	- 해보고 싶었던걸 마음대로 구현해 볼 수 있었다.
	- 내가 하고싶을때만 할 수 있다는 점
- 단점
	- 혼자하려니까 뭘 어디부터 시작 해야할지 막막해서 힘들었다.
	- 프로젝트에 대해서 하려는 동기가 잘 안생긴다.
---

<!--
_color: #333
_backgroundColor: #fff
_backgroundImage: ()
-->

![bg left:39%](https://thumbs.gfycat.com/GenuineBeautifulAnkolewatusi.webp)
# 감사합니다.

<br/>
<br/>
<br/>
<br/>
<br/>

### -끝-
