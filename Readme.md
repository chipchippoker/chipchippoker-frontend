# chipchippoker

- 배포 URL : https://chipchippoker.shop/
- Test ID : yoon1234
- Test PW : password123!

## 프로젝트 화면
### 게임 화면
<img src="https://github.com/yebin113/django_prac/assets/139421100/c96be5e8-b50b-404d-8e02-0d12e43607cb" width="500px" height="300px"/>
<img src="https://github.com/yebin113/django_prac/assets/139421100/23550ec4-f4e7-452a-a6b1-51f3821993ba" width="500px" height="300px"/>
<img src="https://github.com/yebin113/django_prac/assets/139421100/dc2f243b-87ec-4a0b-9618-b1ff17221288" width="500px" height="300px"/>

### 랭킹 화면
<img src="https://github.com/yebin113/django_prac/assets/139421100/60be6245-792e-49d3-9cfb-b4a68cea0bd6" width="500px" height="300px"/>

### 가이드북
<img src="https://github.com/yebin113/django_prac/assets/139421100/1f603298-32c3-415e-a877-a574cd2efab4" width="500px" height="300px"/>

### 프로필 화면
<img src="https://github.com/yebin113/django_prac/assets/139421100/4503e271-1151-4679-8f8a-b993482ca0ed" width="500px" height="300px"/>

```sh
npm install
```

### Compile and Hot-Reload for Development

```sh
npm run dev
```

### Compile and Minify for Production

```sh
npm run build
```
---
### 참여자 명단

- 김대원
- 윤예빈
- 최현기

### 기술스택
- Vue 3.3.11
- Vue-router 4.2.5
- Openvidu-browser 2.29.1
- webstomp-client 1.2.6
- face-api.js 0.22.2

### 역할
- 김대원
    - Openvidu를 사용한 비디오 캠 기능
    - 관전 기능
    - 방 입장, 방 나가기 기능
- 윤예빈
    - WebStomp를 활용한 게임 기능
    - 실시간 친구 신청 기능
    - 감정 인식 기능
    - UI, UX 디자인, CSS
- 최현기
    - WebStomp를 활용한 게임 기능
    - 매칭 기능
    - 토큰 재발행 기능
    - 소셜 로그인 기능
    - CSS

### UI/UX 디자인 (Figma)

<img src="https://github.com/yebin113/django_prac/assets/139421100/077d9c39-4b0a-43f3-8e88-1165e2a8081b" width="500px" height="500px"/>


### Logic Flow
<img src="https://github.com/yebin113/django_prac/assets/139421100/ae498cfa-6f09-40a5-943f-2d5c10fb6f4f" width="500px" height="300px"/>



### 컴포넌트 설계도
<img src="https://github.com/yebin113/django_prac/assets/139421100/6cf09a57-349c-41f2-a262-7cb98224c761" width="500px" height="300px"/>


### 프로젝트 구조
```
📦src
 ┣ 📂components
 ┃ ┣ 📂Cam
 ┃ ┃ ┣ 📜OvVideo.vue
 ┃ ┃ ┗ 📜UserVideo.vue
 ┃ ┣ 📂Main
 ┃ ┃ ┣ 📂Friend
 ┃ ┃ ┃ ┣ 📜MainFriendItem.vue
 ┃ ┃ ┃ ┗ 📜MainFriendList.vue
 ┃ ┃ ┣ 📂Rank
 ┃ ┃ ┃ ┣ 📜MainRank.vue
 ┃ ┃ ┃ ┣ 📜MainRankAllList.vue
 ┃ ┃ ┃ ┣ 📜MainRankFriendList.vue
 ┃ ┃ ┃ ┗ 📜MainRankItem.vue
 ┃ ┃ ┗ 📂Room
 ┃ ┃ ┃ ┣ 📜MainRoom.vue
 ┃ ┃ ┃ ┣ 📜MainRoomFriendList.vue
 ┃ ┃ ┃ ┣ 📜MainRoomItem.vue
 ┃ ┃ ┃ ┗ 📜MainRoomRankList.vue
 ┃ ┣ 📂Modal
 ┃ ┃ ┣ 📂Guide
 ┃ ┃ ┃ ┣ 📜guide1.vue
 ┃ ┃ ┃ ┣ 📜guide2.vue
 ┃ ┃ ┃ ┣ 📜guide3.vue
 ┃ ┃ ┃ ┣ 📜guide4.vue
 ┃ ┃ ┃ ┗ 📜guide5.vue
 ┃ ┃ ┣ 📜ModalCreateRoom.vue
 ┃ ┃ ┣ 📜ModalEnterPassword.vue
 ┃ ┃ ┣ 📜ModalFindFriend.vue
 ┃ ┃ ┣ 📜ModalFindGame.vue
 ┃ ┃ ┣ 📜ModalFindRoom.vue
 ┃ ┃ ┣ 📜ModalGuide.vue
 ┃ ┃ ┣ 📜ModalIconItem.vue
 ┃ ┃ ┣ 📜ModalIconList.vue
 ┃ ┃ ┣ 📜ModalIsExistRoom.vue
 ┃ ┃ ┣ 📜ModalIsFullRoom.vue
 ┃ ┃ ┣ 📜ModalIsPlayingRoom.vue
 ┃ ┃ ┣ 📜ModalLogOut.vue
 ┃ ┃ ┣ 📜ModalMainSettings.vue
 ┃ ┃ ┣ 📜ModalNotExistRoom.vue
 ┃ ┃ ┣ 📜ModalNotificationItem.vue
 ┃ ┃ ┣ 📜ModalNotificationList.vue
 ┃ ┃ ┗ 📜ModalSignOut.vue
 ┃ ┣ 📂Play
 ┃ ┃ ┣ 📜PlayBatting.vue
 ┃ ┃ ┣ 📜PlayController.vue
 ┃ ┃ ┣ 📜PlayEmotion.vue
 ┃ ┃ ┣ 📜PlayEmotionChart.vue
 ┃ ┃ ┣ 📜PlayPlayer.vue
 ┃ ┃ ┗ 📜PlayTalk.vue
 ┃ ┣ 📂Profile
 ┃ ┃ ┣ 📜ProfileHistoryList.vue
 ┃ ┃ ┗ 📜ProfileMyInfo.vue
 ┃ ┗ 📂Wait
 ┃ ┃ ┗ 📜WaitWatcher.vue
 ┣ 📂router
 ┃ ┗ 📜index.js
 ┣ 📂stores
 ┃ ┣ 📜friend.js
 ┃ ┣ 📜game.js
 ┃ ┣ 📜match.js
 ┃ ┣ 📜openvidu.js
 ┃ ┣ 📜room.js
 ┃ ┣ 📜sound.js
 ┃ ┗ 📜user.js
 ┣ 📂views
 ┃ ┣ 📜KakaoSignupView.vue
 ┃ ┣ 📜LoginView.vue
 ┃ ┣ 📜MainView.vue
 ┃ ┣ 📜PlayView.vue
 ┃ ┣ 📜ProfileView.vue
 ┃ ┣ 📜SignupView.vue
 ┃ ┗ 📜WaitView.vue
 ┣ 📜App.vue
 ┣ 📜main.js
 ┗ 📜style.css
 ```



