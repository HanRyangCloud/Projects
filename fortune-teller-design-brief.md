# 점술사 캐릭터 디자인 브리프 (v0.1)

화풍 목표: 스타레일/명조풍 애니 가챠 게임 캐릭터 (셀 셰이딩, 깔끔한 선, 강한 실루엣, 디테일한 의상).
참고 자료는 `fortune-teller-references.md` 참조. 이 브리프는 제가 잡은 초안이며 시안을 보고 수정합니다.

## 공통 설정

- 성별/나이대: 여성, 20대 중반 외모
- 성격 컨셉: 차분하고 신비롭지만 가끔 장난기 있는 상담가. 카드를 뒤집기 전 한쪽 눈썹을 올리는 버릇.
- 시그니처 소품: 공중에 떠서 천천히 도는 타로 카드 3~5장 + 작은 수정구 (손에 쥐지 않고 곁에 떠 있음)
- 대표 모티프: 초승달(여사제 도상), 두 개의 기둥 문양, 베일
- 피해야 할 것: 머릿수건+큰 링 귀걸이+술 달린 숄 같은 "집시 점술사" 클리셰, 실존 캐릭터와 닮은 디자인
- 2D 게임 활용: 전신 일러스트(스플래시 아트), 상반신 대사창 스프라이트, 표정 변화 6종

## 시안 방향 3종

### A. 문 프리스티스 (Waite–Smith 클래식)
- 팔레트: 짙은 남색 + 은색 + 연한 청백색, 포인트로 따뜻한 촛불 노란색
- 의상: 길게 흐르는 푸른 로브, 초승달 머리 장식, 투명한 베일, 두 기둥 문양을 새긴 허리 패널
- 머리: 은빛이 도는 긴 흑발 또는 짙은 남빛 머리, 반묶음
- 분위기: 고요, 신비, 차분

### B. 골드 누보 (아르누보 장식)
- 팔레트: 와인색(버건디) + 금색 + 크림, 포인트로 청록
- 의상: 곡선적인 금 장식이 들어간 코르셋형 드레스 위에 짧은 망토, 꽃과 별이 엮인 헤일로 장식
- 머리: 높게 올린 머리 + 길게 내려오는 땋은 머리
- 분위기: 우아, 화려, 카드 프레임과 잘 어울림

### C. 어반 오라클 (현대 도시형)
- 팔레트: 검정 + 보라 + 시안 네온 포인트, 금색 소량
- 의상: 비대칭 롱코트, 테크웨어풍 벨트와 스트랩, 카드 모양 홀로그램 장식, 짧은 치마와 부츠
- 머리: 단발 + 한쪽만 길게 땋은 머리, 별 모양 헤어핀
- 분위기: 쿨, 도시적, 장난기

## 생성 계획

| 구분 | 내용 |
|---|---|
| 도구 | Gemini 이미지 생성, GPT 이미지 생성 |
| 시안당 | 전신 1장 + 상반신 1장 (A/B/C 각각) |
| 서비스당 장수 | 6장 (3방향 × 2구도) |
| 추가 | 마음에 드는 방향 고르면 표정 시트, 컬러 바리에이션, 턴어라운드 |
| 저장 위치 | `concepts/gemini/`, `concepts/gpt/` |

## 붙여넣기용 프롬프트 (Gemini / ChatGPT 공통)

게임 이름이나 실존 캐릭터 이름은 넣지 않고 특징만 묘사했습니다. 이름을 넣으면 거절되거나 기존 캐릭터와 비슷하게 나올 수 있습니다.

### 공통 스타일 블록 (모든 프롬프트 맨 앞에 붙임)

```
Anime-style gacha game character illustration, polished cel-shaded rendering with soft gradients,
clean confident line art, strong readable silhouette, highly detailed costume with layered fabrics
and metallic ornaments, subtle rim light, plain soft gradient background, single character,
young adult woman fortune teller, floating tarot cards orbiting her, small crystal ball floating beside her.
No text, no watermark.
```

### A. 문 프리스티스
```
[공통 스타일 블록]
Design A "Moon Priestess": long flowing deep-blue robe with silver trim, crescent-moon headpiece,
sheer veil, waist panel with a twin-pillar emblem, long dark hair with a silver sheen, calm mysterious
expression, palette of midnight navy, silver and pale blue with warm candle-yellow accents.
Shot: full body, standing pose, three-quarter view.
```
```
[공통 스타일 블록]
Design A "Moon Priestess" (same design as above). Shot: bust-up portrait facing the viewer,
visual novel dialogue sprite style, neutral calm expression, hands raised holding one tarot card.
```

### B. 골드 누보
```
[공통 스타일 블록]
Design B "Gilded Nouveau": corset-style dress with curving gold Art Nouveau ornaments under a short cape,
halo ornament woven from flowers and stars, hair in a high updo with a long braid falling over the shoulder,
palette of burgundy, gold and cream with teal accents, elegant and ornate.
Shot: full body, standing pose, three-quarter view.
```
```
[공통 스타일 블록]
Design B "Gilded Nouveau" (same design as above). Shot: bust-up portrait facing the viewer,
visual novel dialogue sprite style, gentle smile, one hand lifting a tarot card toward the viewer.
```

### C. 어반 오라클
```
[공통 스타일 블록]
Design C "Urban Oracle": asymmetrical long coat with techwear straps and belts, holographic card-shaped
accessories, short skirt and boots, short bob with one long braid on one side, star-shaped hairpin,
palette of black, purple and cyan neon with a little gold, cool and playful.
Shot: full body, dynamic pose, three-quarter view.
```
```
[공통 스타일 블록]
Design C "Urban Oracle" (same design as above). Shot: bust-up portrait facing the viewer,
visual novel dialogue sprite style, playful smirk with one eyebrow raised, flipping a tarot card.
```

### 사용 팁
- 같은 방향의 전신과 상반신을 한 대화창에서 이어서 뽑으면 얼굴과 의상이 비슷하게 유지됩니다.
- 마음에 드는 시안이 나오면 그 이미지를 첨부하고 "같은 캐릭터로 표정 6종 시트" 식으로 이어 요청하세요.
