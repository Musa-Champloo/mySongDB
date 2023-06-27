# song backup db
mmd motion and camara back up database.  
someof songs has lyrics file (`.lrc`).

# images
This `images` folder stores the cover image of MP3 files.  
(It's useless except for the list view. And it's updated asynchronically.)

# upload guide (ko)
업로드 할 곡 예시:
`ロキ - ナナヲアカリ.mp3`,
`ロキ.mp3`  
파일명을 이렇게 해야되는 이유<sup id="a1">[[1]](#f1)</sup>

1. 엘범이여도 단독이라도 폴더를 생성.  
2. 그 후 [info.json](./info.json) 을 편집.

```json
{
    "f": "ロキ",
    "m": [
        "ロキ/ロキ.mp3",
        "ロキ/ロキ - ナナヲアカリ.mp3"
    ],
    "artist": "MIKU",
    "another": [
        "NANAOAKARI"
    ],
    "tags": [
        "MIKU",
        "VOCALOID",
        "NANAOAKARI"
    ],
    "raw": true,
    "r": 3
}
```
#### 필수
- `f` : 일본어 혹은 영어로 곡명 혹은 앨범명을 작성.
- `m` : 하위 파일구조
- `"raw": true` : 압축파일 인지 아닌지 표기
- `"r": 3` : 저장소 번호

#### 비 필수
- `tags` : 파일 검색, 분류에 쓰이는 태그들.
- `artist` : 메인파일의 아티스트
- `another` : 추가파일의 아티스트
- `maker` : 보컬트레이너, 레이블(엘범) 아티스트
- `atrys` : 커버파일 검색 시도 리스트

# license
This db is made for educational and research purpose.
### Note: maybe somefiles will delete with the original author's objection.

# footnote’s (각주)
<b id="f1">1</b> : 이름이 겹칠때 쓰는걸 권장하며, 가급적 "-" 로 분리표시 하는건 하지 말아주세요.  