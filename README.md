# Django, AWS EC2, uWSGI, nginx

## uWSGI, nginx 배포 참고 싸이트

https://nerogarret.tistory.com/

### 해결중인 오류
1. 입력 명령어 : pip install -r requirements.txt 

오류 : ERROR: Could not install packages due to an OSError: [Errno 2] No such file or directory: '/home/ktietz/src/ci/alabaster_1611921544520/work'

발생 원인 : (불확실) python PATH 문제일 가능성이 있다고 함.

해결 방법 : 우선 필수 모듈만 pip 로 직접 설치.

2. 입력 명령어 : sudo systemctl restart nginx

오류 : nginx: [emerg] invalid number of arguments in "charset" directive in /etc/nginx/sites-enabled/mysite.conf:5

발생 원인 : 오타

해결 방법 : 오타 수정
