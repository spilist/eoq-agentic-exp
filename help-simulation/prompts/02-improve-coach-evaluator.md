`.claude/agents/run-coach-evaluation.md` 와 `.claude/agents/synthesize-evaluation.md`를 분석해서 `coach-response-generator` 와 `coach-response-evaluator` 에이전트를 만들었다.

1. 새로 만든 에이전트들의 내용을 읽고 적절히 한글로 번역해서 내용을 업데이트한다.

2. `commands/evaluate-coach.md`가 새로 만든 에이전트들을 호출해서 기존 의도와 유사하게 병렬로 결과물을 만들 수 있도록 한다. 이를 위해 `.claude/agents/run-coach-evaluation.md` 와 `.claude/agents/synthesize-evaluation.md`를 읽고, `commands/evaluate-coach.md`에 내용을 반영한 뒤, `.claude/agents/run-coach-evaluation.md` 와 `.claude/agents/synthesize-evaluation.md`를 삭제한다.

---

궁금한게 있어. evaluate-coach.md 의 내용 2단계에서, 이미 coach-response-generator 에이전트가 모든 내용을 다 가지고 있는데 prompt를 또 넣는 이유가 뭐지? 프롬프트 버전 번호와 테스트 케이스 인덱스 딱 2개만 넣으면 되는 거 아닌가?

---

좋아. 마찬가지로 3단계도 수정해줘.