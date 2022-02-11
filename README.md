let's make something funny to escape frrom this shitty company

# 초안
빡치는 일 생길 때 마다 접속해서 빡치게 한 사람 이름 제출

이름 제출된 횟수 카운트 해서 카운트가 늘 수록 나무가 점점 자라는거 보여주기


# window 에서 개발환경 설정

로컬에 node js 설치하삼
nodejs.org 접속 후 다운


<cmd오픈>

    node -v

    npm install express-generator -g

<설치 확인>

    express --version


<디렉터리에서 터미널 실행>

    npm start

<웹 브라우저에서 입력>

localhost:3000



# 컨테이너 개발환경 
<소스코드 다운로드>

    git clone <깃헙 주소>


원하는 디렉터리에 소스코드 다운로드

<디렉터리에서 터미널 오픈>

(중요)로컬환경에 도커가 설치된 상태여야함

    docker build . -t <원하는 이미지 이름>

이러면 컨테이너 이미지가 생성됨

생성된 이미지를 가지고 컨테이너를 생성해줄거임

    docker run -p 49160:3000 -d <아까 정한 이미지 이름>

이미지 이름(태그)를 바탕으로 컨테이너 내부 포트(3000)와 로컬 환경 포트(49160, 아무거나 해도 됨)를 포트 바인딩해서 컨테이너 생성


이제 로컬 웹 브라우저에서 localhost:<아까 설정한 포트>로 접속하면

짜잔🙌

컨테이너에 올라간 노드 서버가 동작하는 것을 볼 수 있음