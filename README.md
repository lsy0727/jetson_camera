# jetson_camera

# 설명

https://github.com/lsy0727/jetson_camera/blob/12984477f107a4686e72bb02c8e48d37a2452e42/main.cpp#L7-L14

jetson CSI카메라는 리눅스 드라이버에서 지원하지 않기 때문에 gstreamer명령어를 이용해 영상을 읽음.

src = 카메라를 초기화 하는 명령어 저장

-> 프레임, 영상 크기 등 정보 기입

VideoCapture 생성자의 인자로 gstreamer 명령어를 전달함.


https://github.com/lsy0727/jetson_camera/blob/8df56a53cf3aae188d292274047f3c2a0b027571/main.cpp#L16-L21

dst1 = gstreamer를 이용해 네트워크로 전송하는 명령어 저장(203.234.58.164 / 포트 : 8001)

-> 호스트의 주소와 포트번호를 기입

VideoWriter 생성자에 gstreamer 명령어 전달


https://github.com/lsy0727/jetson_camera/blob/740bbb4227c980ab7084056864f26b1e960a76b5/main.cpp#L40-L52

TickMeter 클래스를 이용해 시간을 출력함.

영상을 gray, 이진화 영상으로 변환하여 출력함.

# 실행 결과
![image](https://github.com/user-attachments/assets/b4d3a10f-d37d-4c77-abe2-1a3e11705162)
