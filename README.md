# kmou-fint.github.io

FINT (Fluid dynamics and Intelligent Navigation Technologies) Lab, Korea Maritime & Ocean University
— 국립한국해양대학교 항해융합학부 김대정·이희진 교수 공동연구실 홈페이지

사이트 주소: https://kmou-fint.github.io

## 파일 구성

```
index.html          홈페이지 전체 (화면 구성 + 내용 데이터)
img/kmou_logo.png   상단 메뉴의 한국해양대 로고
img/campus.jpg      첫 화면 캠퍼스 사진
img/                구성원 사진, 수상·소식 사진을 넣는 폴더
```

## 내용 수정하기

`index.html` 안의 `<script>` 맨 위, **✏️ 내용 수정은 여기서만 하면 됩니다** 부분만 고치면 됩니다.

| 항목 | 고칠 곳 |
|---|---|
| 연구실 소개, 첫 화면 문구 | `LAB` |
| 첫 화면 캠퍼스 사진과 설명 | `LAB.heroPhoto`, `LAB.heroPhotoCaption` |
| 연구 분야, 공동 연구 | `AREAS`, `JOINT` |
| 수행 과제 | `PROJECTS` |
| 구성원 | `MEMBERS` |
| 논문·특허 | `PUBS` |
| 수상 | `AWARDS` |
| 소식 | `NEWS` |

- `[과제명]`처럼 `[`로 시작하는 항목은 화면에 나오지 않습니다.
- 첫 화면 사진은 `img/campus.jpg`입니다. 같은 구도의 고해상도 원본을 같은 이름으로 올리면 그대로 더 선명해집니다. 사진 위 주석(아치섬, 실습선 부두)과 흐름선은 이 사진 구도에 맞춰져 있습니다.
- 사진은 `img` 폴더에 올리고 `photo: "img/파일명.jpg"`처럼 경로를 적습니다.
- 논문의 `jcr`에 JCR 백분위를 넣으면 논문 통계 그래프에 자동으로 반영됩니다.
- 사이트 색을 바꾸려면 `<style>` 맨 위 `:root`의 값을 고칩니다.

GitHub에서 파일을 수정하고 커밋하면 1~2분 뒤 사이트에 반영됩니다.
