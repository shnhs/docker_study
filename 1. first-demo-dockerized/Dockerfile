# 컨테이너에서 nodeJS를 사용하기 위함
FROM node:14

# 컨테이너 자체 파일 시스템 디렉토리
WORKDIR /app

# 해당 파일을 복사해라
COPY package.json .

# npm 명령을 실행하여 애플리케이션에 필요한 요소를 설치
RUN npm install

# 나머지 코드를 여기에 복사해라
COPY . .

# 외부포트 3000번으로 실행
EXPOSE 3000

# node 명령어로 실행
CMD [ "node", "app.mjs" ]