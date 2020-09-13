1. 프로젝트 폴더 생성 & 이동
```
mkdir project
cd project
```

2. 가상환경 생성
```
pyenv virtualenv 버전(ex.3.8.5) project-env
```

3. 가상환경 적용
```
pyenv local project-env
```

4. 장고 설치
```
pip install django
```

5. 프로젝트 생성
```
django-admin startproject config
```

6. 설치된 패키지들을 requirement.txt에 기록
```
pip freeze > requirements.txt
```

7. app 추가
```
./manage.py startapp app
```

가상환경 삭제
```
pyenv virtualenv-delete project-env
```
