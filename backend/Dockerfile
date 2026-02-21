# 1. 파이썬 3.9 버전을 기반으로 시작합니다.
FROM python:3.9-slim

# 2. 컨테이너 내부의 작업 폴더를 /app으로 정합니다.
WORKDIR /app

# 3. (나중에) 백엔드 개발자가 줄 requirements.txt를 복사해서 패키지를 설치합니다.
# 지금은 파일이 없으니 주석 처리해 둡니다.
# COPY requirements.txt .
# RUN pip install -r requirements.txt

# 4. 백엔드 소스 코드를 모두 복사합니다.
COPY . .

# 5. 서버가 8000번 포트를 쓴다고 도커에게 알려줍니다.
EXPOSE 8000

# 6. 서버 실행 명령어 (임시로 서버가 꺼지지 않게 무한 대기 명령어를 넣습니다)
# 나중에 팀원이 코드를 주면 CMD ["python", "main.py"] 등으로 바꿉니다.
CMD ["tail", "-f", "/dev/null"]
