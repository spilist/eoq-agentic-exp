resources/행동계획-코치-v[0-9].md가 충분히 적절하게 행동계획을 코칭해주는지 판단할 수 있는 테스트 데이터 셋을 evaluatoin/case-[1-4]에 만들었어.

1. 지금 각 디렉토리에 input-text.md 로 들어있는 내용 중 checklist에 해당하는 내용만 남겨서 각 디렉토리에 checklist.md 로 바꿔줘.

2. `행동계획-코치`를 4가지 케이스에 대해 병렬로 평가하는 서브에이전트를 만들어줘. 
- 입력: 버전 몇이냐 (행동계획-코치-v0, -v1, ...)
- 출력: 각 case에 대해 병렬로 input-text를 입력으로 해서, 그 응답을 /evaluation/results 에 YYMMDD-{index}-case{n}.md 으로 저장한다.

3. '2에서 만든 서브에이전트들을 돌려서 다음과 같은 결과를 내는 메인 에이전트'를 위한 프롬프트를 만들어줘.
- /evaluation/results/YYMMDD-{index}-case{n}.md 를 모두 읽는다.
- 결과를 종합하여 /evaluation/results/YYMMDD-{index}-종합.md 에 기록한다.