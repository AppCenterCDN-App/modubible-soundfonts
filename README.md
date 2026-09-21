# ModuBible Soundfonts

모두의 성경(ModuBible) 앱의 찬송 반주용 **피아노 사운드폰트**를 배포하는 곳입니다. 앱은 GeneralUser GS 의
피아노를 동봉하고, 더 좋은 피아노 소리를 원하는 사용자가 아래 것을 내려받아 바꿔 쓸 수 있습니다.
파일은 [Releases](../../releases) 에 있습니다. 모두 **SF3**(SoundFont 2 구조에 샘플만 Ogg Vorbis 로 압축)이며,
FluidSynth·TinySoundFont 등 SF3 를 읽는 신시사이저에서 그대로 씁니다.

Piano soundfonts redistributed for the ModuBible (모두의 성경) Android app. All files are **SF3** (SoundFont 2
structure with Ogg Vorbis–compressed samples), readable by FluidSynth, TinySoundFont and other SF3-aware synthesizers.

| 파일 | 원본 | 라이선스 | 크기 |
|---|---|---|---|
| `piano-upright-kw.sf3` | [Upright Piano KW](https://freepats.zenvoid.org/Piano/acoustic-grand-piano.html) (FreePats, 2022-02-21) | CC0 1.0 | 5.4MB |
| `piano-ydp-grand.sf3` | [YDP Grand Piano](https://freepats.zenvoid.org/Piano/acoustic-grand-piano.html) (FreePats, 2016-08-04) | CC BY 3.0 | 13.7MB |
| `piano-salamander.sf3` | [Salamander Grand Piano V3](https://freepats.zenvoid.org/Piano/acoustic-grand-piano.html) (Alexander Holm / FreePats, 2020-06-02) | CC BY 3.0 | 125MB |

원본 제작자와 라이선스 전문은 [`licenses/`](licenses/) 에 그대로 두었습니다. 우리가 한 일은 SF2 → SF3 변환
(샘플을 Vorbis q6 로 압축)뿐이며, 음·루프·프리셋은 원본 그대로입니다. 변환 도구는 ModuBible 저장소의
`tools/hymn/sf2_to_sf3.py` 입니다.

## 앱이 읽는 목록

[`manifest.json`](manifest.json) 이 파일마다 주소·크기·SHA-256 을 담습니다. 앱은 이 목록을 읽어 내려받고
검증합니다. 새 판을 올릴 때는 릴리스를 새로 만들고 목록의 `version` 을 올립니다.

## Attribution

- Upright Piano KW — see `licenses/UprightPianoKW-readme.txt` (FreePats project, CC0 1.0).
- YDP Grand Piano — roberto@zenvoid.org for the FreePats project, CC BY 3.0.
- Salamander Grand Piano — Alexander Holm, CC BY 3.0; SF2 packaging by the FreePats project.
