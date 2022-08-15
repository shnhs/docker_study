# base가 될 운영체제 이미지
FROM node

# 명령어들이 실행될 경로 지정
WORKDIR /app 

COPY package.json /app

# 필요한 명령어 입력
RUN npm install

# 앞은 컨테이너 외부 경로 - . 이라면 Dockerfile이 포함된 경로의 모든 하위 소스
# 뒤에는 컨테이너 내부 경로, ./ 라면 현재 작업경로로 지정
COPY . /app

# 특정 포트에 노출 세팅
EXPOSE 80

# 이미지 기반의 컨테이너가 생성될 때 마다 해당 명령어 실행 
CMD [ "node", "server.js" ]
