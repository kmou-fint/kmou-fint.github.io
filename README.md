# kmou-fint.github.io

FINT (Fluid dynamics and Intelligent Navigation Technologies) Lab, Korea Maritime & Ocean University
— 국립한국해양대학교 항해융합학부 김대정·이희진 교수 공동연구실 홈페이지

사이트 주소: https://kmou-fint.github.io

## 파일 구성

```
index.html          홈페이지 전체 (화면 구성 + 내용 데이터)
img/kmou_logo.png   상단 메뉴의 한국해양대 로고
img/campus.jpg      첫 화면 캠퍼스 사진
papers/             논문 PDF (파일 이름 = 논문 제목)
video/scenario.mp4  공동 연구 영상 (img/scenario_poster.jpg 는 재생 전 보이는 첫 화면)
img/                구성원 사진, 수상·소식 사진을 넣는 폴더
```

## 내용 수정하기

`index.html` 안의 `<script>` 맨 위, **✏️ 내용 수정은 여기서만 하면 됩니다** 부분만 고치면 됩니다.

| 항목 | 고칠 곳 |
|---|---|
| 연구실 소개, 첫 화면 문구 | `LAB` |
| 첫 화면 캠퍼스 사진과 설명 | `LAB.heroPhoto`, `LAB.heroPhotoCaption` |
| 연구 분야, 공동 연구 | `AREAS`, `JOINT` |
| 공동 연구 영상과 설명 | `JOINT.video` |
| 수행 과제 | `PROJECTS` |
| 구성원 | `MEMBERS` |
| 논문·특허 | `PUBS` |
| 수상 | `AWARDS` |
| 소식 | `NEWS` |

- `[과제명]`처럼 `[`로 시작하는 항목은 화면에 나오지 않습니다.
- 첫 화면 사진은 `img/campus.jpg`(가로 2560px)입니다. 사진 위 주석(아치섬, 실습선 부두)과 흐름선은 이 사진 구도에 맞춰져 있습니다.
- **사진·로고 같은 이미지 파일은 연필(Edit) 버튼으로 이름을 바꾸거나 옮기지 마세요.** 파일이 깨집니다. 옮길 때는 원하는 폴더에 들어가서 Upload files로 다시 올리세요.
- 영상은 **H.264 형식의 mp4**여야 모든 브라우저에서 재생됩니다. 아이폰 등에서 찍은 HEVC(H.265) 영상은 크롬에서 안 나올 수 있으니 변환해서 올리세요.
- 사진은 `img` 폴더에 올리고 `photo: "img/파일명.jpg"`처럼 경로를 적습니다.
- 논문의 `jcr`에 JCR 백분위를 넣으면 논문 통계 그래프에 자동으로 반영됩니다.
- 사이트 색을 바꾸려면 `<style>` 맨 위 `:root`의 값을 고칩니다.

GitHub에서 파일을 수정하고 커밋하면 2~3분 뒤 사이트에 반영됩니다.

### 자동 배포 (`.github/workflows/deploy.yml`)

커밋할 때마다 **Actions** 탭의 "Deploy site"가 자동으로 실행되어, 화면에 그려지는 글(연구 분야·구성원·논문 목록 등)을 `index.html` 안에 미리 써 넣은 뒤 배포합니다. 그래서 코드를 실행하지 않는 검색 로봇(네이버 등)도 내용을 읽을 수 있습니다.
- 이 기능을 쓰려면 **Settings → Pages → Build and deployment → Source** 가 **GitHub Actions** 로 되어 있어야 합니다.
- 저장소의 `index.html` 은 바뀌지 않으니 지금처럼 데이터 부분만 고치면 됩니다.
- 반영이 안 되면 Actions 탭에서 빨간 X가 있는지 확인하세요.

## 논문 PDF 다운로드 버튼

1. 저장소에 `papers` 폴더를 만들고 PDF를 올립니다.
2. **파일 이름은 논문 제목 그대로** 두면 됩니다. 예) `Navigating narrow waterways A quantitative study on timing of stand-on ship actions.pdf`, `합성 LSTM 모델을 활용한 선박 항적 예측.pdf`
   - 대소문자, 띄어쓰기, 문장부호(`:` `,` `-` 등)는 달라도 됩니다. 제목이 길면 앞부분(20자 이상)만 있어도 됩니다.
3. 1~2분 뒤 새로고침하면 그 논문 옆에 **PDF 다운로드** 버튼이 생깁니다. 방문자가 받으면 `저자 (연도) 제목.pdf` 이름으로 저장됩니다.

내려받은 이름 그대로(예: `1-s2.0-S0029801825001155-main.pdf`) 올리고 싶으면, `PUBS`에서 그 논문의 `pdf:""` 칸에 파일 이름을 적어 주면 됩니다.
