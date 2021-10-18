    1) react를 설치한다. npx create-react-app .
    2) npm i concurrently wait-on -D
    3) script에 아래의 실행을 넣어 둔다.
    	"electron:start": "wait-on http://localhost:3000 && electron .",
    	"both": "concurrently \"npm run start\" \"npm run electron:start\""
    4) "main": "public/electron.js"을 package.js에 추가한다.
    5) npm run both를 실행해서 잘 작동하는지 테스트를 한다.
    
    리액트 관련 참고 사이트 : https://github.com/shmoon2917 
