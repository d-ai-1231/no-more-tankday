## 슬래시 커맨드 설정 (복붙용)

아래 파일을 프로젝트의 `.claude/commands/review-campaign.md`로 복사하면, `/review-campaign` 명령어로 수동 검수를 호출할 수 있다.

```bash
mkdir -p .claude/commands
cp no-more-tankday/setup/review-campaign-command.md .claude/commands/review-campaign.md
```

### 커맨드 파일 내용

```md
아래 캠페인 정보를 no-more-tankday의 marketing-cultural-risk 스킬 기준으로 검토해줘.

검토 기준: skills/marketing-cultural-risk/SKILL.md

검토 항목:
- 캠페인명
- 제품명
- 출시일
- 메인 카피
- 서브 카피
- 비주얼 설명
- 해시태그
- 채널
- 타깃 고객

추가 검토:
- 날짜 + 캠페인명 + 카피 조합 리스크
- 실시간 이슈 (검색 도구가 있으면 최근 3일 이내 뉴스 확인)

출력은 SKILL.md의 출력 형식을 따른다.

---

캠페인 정보:

브랜드: $ARGUMENTS
```

### 사용법

```
/review-campaign 브랜드명
```
