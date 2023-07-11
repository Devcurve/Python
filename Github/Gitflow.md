# **Gitflow**
### Gitflow는 Git을 기반으로 한 효율적인 브랜치 관리 전략중 하나입니다.

**Gitflow의 주요 브랜치**<br>
- Main Branch: 주요 브랜치로서, 안정된 소프트웨어 버전을 관리하는 데 사용됩니다. 보통 "master" 또는 "main"이라는 이름으로 사용됩니다.
- Develop Branch: 개발 브랜치로서, 다음 배포 버전을 준비하는 데 사용됩니다. 기능 개발이나 버그 수정과 같은 작업은 이 브랜치에서 이루어집니다.
- Feature Branch: 새로운 기능을 개발하기 위한 브랜치입니다. Develop 브랜치에서 분기하고 개발이 완료되면 Develop 브랜치로 병합합니다.
- Release Branch: 배포를 준비하기 위한 브랜치입니다. Develop 브랜치의 기능을 안정화하고 버그 수정 및 준비 작업을 수행한 후 Main 브랜치로 병합합니다.
- Hotfix Branch: 긴급한 버그 수정을 위한 브랜치입니다. Main 브랜치에서 분기하고 수정이 완료되면 Main 및 Develop 브랜치로 병합합니다.

---
- Feature: 새로운 기능을 개발하는 Pull Request Label
- Bugfix: 버그 수정을 위한 Pull Request Label
- Hotfix: 긴급한 버그 수정을 위한 Pull Request Label
- Release: 배포 준비를 위한 Pull Request Label
- Documentation: 문서 업데이트를 위한 Pull Request Label
- Refactor: 코드 리팩토링을 위한 Pull Request Label
- Review Needed: 리뷰어들에게 검토를 요청한 Pull Request Label
- Ready for Merge: 병합 가능한 상태의 Pull Request Label
- On Hold: 일시적으로 보류된 Pull Request Label

---
___추가 Label___

- Bug: 버그 수정과 관련된 Pull Request
- Feature: 새로운 기능 추가를 위한 Pull Request
- Enhancement: 기존 기능의 개선을 위한 Pull Request
- Refactor: 코드 리팩토링을 위한 Pull Request
- Tests: 테스트 작성 또는 수정을 위한 Pull Request
- WIP (Work in Progress): 작업 중인 Pull Request
