# config in-project
[가상환경 프로젝트 내부에 생성하기](https://python-poetry.org/docs/configuration/#virtualenvsin-project)
```shell
poetry config virtualenvs.in-project true
```

# init
대화 형식으로 `pyproject.toml` 파일을 생성한다.  
```shell
poetry init
```

# add / remove
```shell
poetry add django
poetry add pytest factory-boy --dev
poetry remove requests
```

# run
가상환경에 설치된 패키지를 실행
```shell
poetry run pytest
poetry run django-admin startproject config .
```

# shell / deactivate
가상환경 모드로 진입
```shell
poetry shell
which django-admin
pytest

deactivate
```

# requirements.txt 파일로 저장하기
[export cli](https://python-poetry.org/docs/cli#export)
```shell
poetry export -f requirements.txt > requirements.txt
```
