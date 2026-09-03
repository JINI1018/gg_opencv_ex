# OpenCV 기본

# github repository 생성
- git clone 하기
- 작업 디렉토리로 이동
```
cd opencv_py_ex
```

# 가상환경 만들기
- PowerShell에서 스크립트 실행 허용(한번도 실행 안했다면 실행)  
```
Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
```
- 가상환경 만들기
```
uv init --bare --python 3.12 --name yolo-ex
uv python pin 3.12
```

# 주피터 노트북 환경만들기
```
uv add ipykernel
uv run python -m ipykernel install --user --name .venv
```

# 라이브러리 설치
```
uv add "opencv-python==4.12.0.88"
```

# jpyter lab 사용시 
- jupyterlab 설치
```
uv add jupyterlab
```

- jupyterlab 실험
```
uv run jupyter lab
```

# 실습 내용 정리

| 파일 | 실습 내용 |
|---|---|
| 21openCVimageConvert.py | 이미지 읽기 → 그레이스케일 변환 |
| 22openCVimage.py | 이미지 정보(shape) 출력, 흑백 변환 후 파일 저장(imwrite) |
| 23openCVimagePixel.py | 픽셀 값 접근(BGR), 영역 슬라이싱/색 채우기 |
| 24openCVDraw.py | 사각형·원·선·텍스트 그리기 |
| 25openCVImage.py | 이동/회전/리사이즈(주석) + 대칭(flip) |
| 26openCVMasking.py | 원형 마스크 생성, bitwise_and 마스킹 |
| 27openCVChannel.py | 채널 분리(split)/병합(merge), 색공간 필터(주석) |