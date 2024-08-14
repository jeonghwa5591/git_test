### 과제 
### 빅 데이터 연습 
#### 마크다운 연습을 하려면 다음 사이트로 가면됩니다.[html](https://www.heropy.dev/p/B74sNE)
### 이미지 
### ![이미지 입니다.](alice_color.png)

### 이미지 읽어오기

import cv2
import matplotlib.pyplot as plt
image=cv2.imread("d:/data/alice_color.png", cv2.IMREAD_COLOR)
# 이미지가 제대로 읽혔는지 확인
if image is None:
    print("이미지를 읽어오는 데 실패했습니다.")
else:
    # 이미지를 RGB로 변환 (OpenCV는 기본적으로 BGR로 이미지를 읽어옴)
    image_rgb = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)

    # 이미지 표시
    plt.imshow(image_rgb)
    plt.axis('off')  # 축 제거
    plt.show()
