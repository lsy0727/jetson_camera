# jetson_camera

# 설명

https://github.com/lsy0727/jetson_camera/blob/12984477f107a4686e72bb02c8e48d37a2452e42/main.cpp#L7-L14

src = 카메라를 초기화 하는 명령어

jetson CSI카메라는 리눅스 드라이버에서 지원하지 않기 때문에 gstreamer명령어를 이용해 영상을 읽음.

-> VideoCapture 생성자의 인자로 gstreamer 명령어를 전달함.

# 실행 결과
![image](https://github.com/user-attachments/assets/b4d3a10f-d37d-4c77-abe2-1a3e11705162)
