# 자유의 여신상 XR 가상전시관

**XR 실습 2 — 가상전시관형 자유의 여신상 탐방**

뉴욕 자유의 여신상을 주제로 한 웹 기반 3D 가상전시관입니다. 관람객이 가상 박물관의 VR·AR·MR 전시실을 찾아가고, 각 전시실에서 실제 체험 페이지를 실행하도록 설계했습니다.

## 체험 주소

GitHub Pages 배포 후 다음 주소에서 관람할 수 있습니다.

https://ilmac-knu.github.io/statue-liberty-museum-xr/

## 전시실 구성

| 전시실 | 체험 내용 | 링크 |
|---|---|---|
| VR 전시관 | 360° 자유의 여신상 탐방 | https://ilmac-knu.github.io/statue-liberty-vr/ |
| AR 설명판 | 카메라로 이미지 인식 후 설명판 표시 | https://ilmac-knu.github.io/season3-ar-plus/ |
| AR 영상 | 카메라로 이미지 인식 후 영상 표시 | https://ilmac-knu.github.io/ar-travel/ |
| MR 배치 | 현실 공간에 3D 자유의 여신상 배치 및 손가락 조작 | https://ilmac-knu.github.io/statue-liberty-touch-mr/ |

## 사용 방법

1. 전시관 페이지에 접속합니다.
2. 화면의 전시대를 클릭하거나 아래의 **로비 / VR / AR / MR** 이동 버튼을 누릅니다.
3. 마우스 또는 손가락으로 화면을 드래그하여 시선을 회전합니다.
4. 화면 아래 전시실 카드에서 해당 **체험** 버튼을 눌러 새 탭에서 콘텐츠를 실행합니다.
5. **처음 위치로** 버튼으로 전시관 로비로 돌아옵니다.

> AR은 카메라 권한과 인식용 자유의 여신상 이미지가 필요합니다. MR 체험도 카메라 권한 및 기기 지원 여부에 영향을 받습니다.

## 기술 및 특징

- HTML, CSS, JavaScript
- Three.js를 활용한 3D 전시 공간(인터넷 연결 시 CDN에서 라이브러리 로드)
- PC와 스마트폰의 마우스/터치 조작 지원
- 전시대 선택 시 카메라 시점 이동
- 외부 체험 링크를 새 탭에서 실행
- 3D 라이브러리를 불러오지 못하더라도 하단 체험 링크 사용 가능
- 별도의 3D 모델 파일이나 이미지 파일 없이 작동하는 기본 전시관

**구분:** 이 프로젝트의 박물관 자체는 웹 기반 3D 가상 공간이며, 실제 VR·AR·MR 체험은 연결된 개별 페이지에서 실행됩니다. 중앙 조형물은 자유의 여신상을 연상시키는 단순화된 전시 조형이며 정밀 복제 모델이 아닙니다.

## GitHub Pages 배포

1. GitHub에서 `statue-liberty-museum-xr` 공개 저장소를 만듭니다.
2. 저장소 최상위에 `index.html`과 `README.md`를 업로드합니다.
3. **Settings → Pages → Build and deployment**로 이동합니다.
4. **Deploy from a branch**를 선택하고 `main` / `/(root)`를 지정하여 저장합니다.
5. 배포가 완료되면 위 체험 주소에 접속합니다.

## 파일 구조

```text
statue-liberty-museum-xr/
├── index.html     # 3D 전시관 및 XR 체험 연결
└── README.md      # 프로젝트 설명 및 배포 안내
```

## 참고

카메라 기반 AR·MR 체험은 스마트폰의 브라우저 및 보안 설정에 따라 작동 여부가 달라질 수 있습니다. 카메라 사용 권한을 허용하고, 각 콘텐츠가 요구하는 인식용 이미지를 준비하세요.
