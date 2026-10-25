<div align="center">


# 춘풍팀 · Team Chunpung (SpringWindsTeam)

**한국어 여론·사회 시뮬레이션을 위한 오픈소스와 데이터**

[![GitHub](https://img.shields.io/badge/GitHub-SpringWindsTeam-181717?logo=github)](https://github.com/SpringWindsTeam)
[![Hugging Face](https://img.shields.io/badge/🤗%20Hugging%20Face-springwindteam-yellow)](https://huggingface.co/springwindteam)
[![Email](https://img.shields.io/badge/email-spring.wind.team%40gmail.com-blue)](mailto:spring.wind.team@gmail.com)

</div>

LLM 페르소나가 한국어로 대화하는 **단톡방 여론 시뮬레이션**을 연구·개발합니다. 국산 AI 모델(EXAONE · A.X · HyperCLOVA X · Solar · Kanana …)과
공개 페르소나 데이터로, 정책·제품·동네 소식에 대한 시민 반응을 대화 기록으로 재현하는 도구를 만듭니다.

## 프로젝트

| 이름 | 무엇 | 설치 |
|---|---|---|
| [**sarangbang**](https://github.com/SpringWindsTeam/sarangbang) 사랑방 | 한국어 단톡방 여론 시뮬레이션 엔진. 국산 모델 제공처 프리셋, 시나리오 JSON, CLI | `pip install sarangbang` |
| [**Nemotron-Personas-Korea 증강판**](https://huggingface.co/datasets/springwindteam/nemotron-personas-korea-augmented) | 한국인 100만 명 합성 페르소나 — 소득 순위·정치 성향·자녀 유무·교육 종사 여부·1인칭 서사 추가 (CC BY 4.0) | `sarangbang.adapters.load_nemotron_rows` |

```bash
pip install sarangbang
sarangbang quickstart --fake              # 네트워크 없이 30초 체험
sarangbang providers                      # 국산 AI를 쓸 수 있는 곳
```

## 원칙

- **엔진에 무작위를 넣지 않는다.** 같은 입력이면 같은 발언 순서·카드 배분. 달라지는 것은 모델 표본 추출뿐.
- **매 호출은 독립이다.** 에이전트 메모리를 쌓지 않고 대화 기록을 매번 다시 렌더한다.
- **국산 모델 우선, 그러나 종속 없음.** OpenAI 호환 서버면 무엇이든 붙는다.
- **합성 데이터만.** 실제 사람의 글·닉네임·프로필을 페르소나로 쓰지 않는다.

## 기여·문의

- 이슈와 PR은 각 저장소의 CONTRIBUTING.md를 따릅니다. 국산 모델 제공처 정보 갱신 이슈를 특히 환영합니다.
- 보안 문제는 공개 이슈 대신 각 저장소의 SECURITY.md 채널로 알려 주세요.
- 연구 협업·데이터 문의: spring.wind.team@gmail.com
