---
title: Github Convention
date: 2023-11-22T23:10:48+09:00
next: docs/convention
prev: docs/convention/study_convention
weight: 3
---
![image](asset/images/git-merge.gif)

해당 페이지에는 Project 555 팀원들이 개발 기간 중 준수했던 Github 과 관련된 규약에 관해 설명합니다.

## Branch
Plog의 Branch 는 다음과 같은 형태로 작성하여야 합니다.

### Fixed Branch
- `main`: 배포용 브랜치, 개발 서버를 배포하는 브런치로, 기능 개발 및 버그 픽스가 완료된 코드가 Merge 되는 Target Branch 입니다.

### Temporary Branch
-  `feat/#{issue_number}`: 기능 개발 브랜치, 기능 개발을 위한 브랜치로, `main` 브랜치로부터 분기되어 개발이 진행되며, 완료 시 `main` 브랜치로 Merge 됩니다.
  - Merge 후에는 해당 브랜치를 삭제합니다.
- `fix/#{issue_number}`: 버그 픽스 브랜치, 버그 픽스를 위한 브랜치로, `main` 브랜치로부터 분기되어 개발이 진행되며, 완료 시 `main` 브랜치로 Merge 됩니다.
  - Merge 후에는 해당 브랜치를 삭제합니다.
- `docs/#{issue_number}`: 문서 작성 브랜치, 문서 작성을 위한 브랜치로, `main` 브랜치로부터 분기되어 개발이 진행되며, 완료 시 `main` 브랜치로 Merge 됩니다.
  - Merge 후에는 해당 브랜치를 삭제합니다.
- `refactor/#{issue_number}`: 리팩토링 브랜치, 리팩토링을 위한 브랜치로, `main` 브랜치로부터 분기되어 개발이 진행되며, 완료 시 `main` 브랜치로 Merge 됩니다.
  - Merge 후에는 해당 브랜치를 삭제합니다.
- `chore/#{issue_number}`: 기타 작업 브랜치, 기타 작업을 위한 브랜치로, `main` 브랜치로부터 분기되어 개발이 진행되며, 완료 시 `main` 브랜치로 Merge 됩니다.
  - Merge 후에는 해당 브랜치를 삭제합니다.
- `test/#{issue_number}`: 테스트 브랜치, 테스트를 위한 브랜치로, `main` 브랜치로부터 분기되어 개발이 진행되며, 완료 시 `main` 브랜치로 Merge 됩니다.
  - Merge 후에는 해당 브랜치를 삭제합니다.

## Commit Message Convention
커밋 메시지는 다음 포맷에 따라 작성합니다.
```
[#{issue_number}] {title}

{description}
```

## Pull Request Convention

### Foramt
Pull Request의 Title은 다음 포멧에 맞추어 작성되어야 합니다. 
```
[#{issue_number}] {title}
```

Pull Request의 Description은 다음 포멧에 맞추어 작성되어야 합니다. 
```md
# 세부 구현
- 한 일 1
- 한 일 2
- 한 일 3
- ...
```

###  Code Review Rule
- 코드 리뷰는 최소 1명 이상의 팀원이 리뷰를 진행합니다.
  - 게시 이후 1일 경과 시, Test 가 통과되었다면 Approve 없이 Merge 를 허용합니다.
- 각 코멘트의 경우 해결 시 Resolve 를 통해 해결합니다. (Resolve 는 리뷰어, 리뷰이 둘 다 가능합니다.)

#### Result
> 코드 리뷰 결과는 다음을 나타내며, 각 결과에 따라 다음과 같은 행동을 취합니다

|Result| Description                                                                                        |
|---|----------------------------------------------------------------------------------------------------|
|`Approve`| 모든 코드가 정상적으로 이행되며, 이상이 없고, 수정사항 없음. _(Merge 허용)_                                                   |
|`Comment`| 코드는 이상이 없으나, 주석 누락, 로직 간략화 등 수정 사항을 제안하거나 코드 관련 질문의 경우 사용. _(약한 수정 권고, 다른 사람의 Approve 후 Merge 허용)_ |
|`Request Change`| 코드를 수정하는 것을 강력히 권고함. _(수정 강제, Merge 불가)_                                                           |

## Merge Strategy
- Pull Request를 통해 `Approve` 수가 **1개 이상**인 경우에 허용합니다. (게시 경과 1일 이후는 예외)
- 커밋이 많은 경우 `Squash`, 커밋이 별로 없고, 각 커밋이 의미를 담고 있는 경우 `Rebase`를 기본 전략으로 합니다.
- Target Branch는 `main` 으로 설정합니다.