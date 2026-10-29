# kmou-fint.github.io

FINT (Fluid dynamics and Intelligent Navigation Technologies) Lab, Korea Maritime & Ocean University
— 국립한국해양대학교 항해융합학부 김대정·이희진 교수 공동연구실 홈페이지

사이트 주소: https://kmou-fint.github.io

## 파일 구성

```
index.html          홈페이지 전체 (화면 구성 + 내용 데이터)
img/kmou_logo.png   상단 메뉴의 한국해양대 로고
img/campus.jpg      첫 화면 캠퍼스 사진
papers/             논문 PDF (아래 파일 이름 목록 참고)
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

GitHub에서 파일을 수정하고 커밋하면 1~2분 뒤 사이트에 반영됩니다.

## 논문 PDF 다운로드 버튼

`papers` 폴더에 아래 이름 그대로 PDF를 올리면 해당 논문 옆에 **PDF** 버튼이 자동으로 생깁니다. 파일이 없는 논문은 버튼이 나오지 않습니다.
새 논문을 추가할 때는 `PUBS`에 `pdf:"papers/파일이름.pdf"`를 적고 같은 이름으로 올리면 됩니다.

| 파일 이름 | 논문 (학술지, 권(호), 쪽) |
|---|---|
| `2025_Lee_KINPR_49-3_352.pdf` | 한국항해항만학회지, 49(3), 352-358 |
| `2025_Lee_KINPR_49-3_286.pdf` | 한국항해항만학회지, 49(3), 286-291 |
| `2025_Lee_KINPR_49-2_153.pdf` | 한국항해항만학회지, 49(2), 153-158 |
| `2025_Lee_KINPR_49-2_173.pdf` | 한국항해항만학회지, 49(2), 173-178 |
| `2025_Lee_KOSOMES_31-2_241.pdf` | 해양환경안전학회지, 31(2), 241-249 |
| `2024_Lee_KOSOMES_30-6_619.pdf` | 해양환경안전학회지, 30(6), 619-625 |
| `2025_Lee_JMSE_13-8_1492.pdf` | Journal of Marine Science and Engineering, 13(8), 1492 |
| `2025_Lee_OE_322_120400.pdf` | Ocean Engineering, 322, 120400 |
| `2024_Lee_OE_294_116766.pdf` | Ocean Engineering, 294, 116766 |
| `2023_Song_OE_279_114602.pdf` | Ocean Engineering, 279, 114602 |
| `2023_Kim_KINPR_47-2_66.pdf` | Journal of Navigation and Port Research, 47(2), 66–74 |
| `2023_Kim_KINPR_47-1_10.pdf` | Journal of Navigation and Port Research, 47(1), 10–17 |
| `2023_Kim_OE_270_113681.pdf` | Ocean Engineering, 270, 113681 |
| `2022_Lee_OE_263_112340.pdf` | Ocean Engineering, 263, 112340 |
| `2022_Lee_JMSE_10-7_859.pdf` | Journal of Marine Science and Engineering, 10(7), 859 |
| `2022_Lee_JMSE_10-10_1420.pdf` | Journal of Marine Science and Engineering, 10(10), 1420 |
| `2022_Lee_JMSE_10-7_961.pdf` | Journal of Marine Science and Engineering, 10(7), 961 |
| `2022_Kim_OE_263_112364.pdf` | Ocean Engineering, 263, 112364 |
| `2022_Kim_OE_256_111492.pdf` | Ocean Engineering, 256, 111492 |
| `2022_Kim_AOR_123_103176.pdf` | Applied Ocean Research, 123, 103176 |
| `2022_Kim_OE_248_110808.pdf` | Ocean Engineering, 248, 110808 |
| `2022_Kim_IJNAOE_14_100425.pdf` | International Journal of Naval Architecture and Ocean Engineering, 14, 100425 |
| `2021_Lee_JoN_74-5_1172.pdf` | The Journal of Navigation, 74(5), 1172–1188 |
| `2021_Kim_AOR_117_102940.pdf` | Applied Ocean Research, 117, 102940 |
| `2021_Kim_OE_237_109615.pdf` | Ocean Engineering, 237, 109615 |
| `2021_Kim_OE_236_109567.pdf` | Ocean Engineering, 236, 109567 |
