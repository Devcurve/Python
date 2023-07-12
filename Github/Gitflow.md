# **Github download**

### [`github desktop download`](https://central.github.com/deployments/desktop/desktop/latest/win32)
###### - download가 안된다면 [link](https://desktop.github.com/)로 이동하여 직접 download 해주세요~
- 설치방법은 생략




### Github를 사용하기 위한 용어 정리.
- `저장소(Repository)`: GitHub에서 프로젝트를 저장하는 공간입니다. 저장소는 파일, 폴더, 코드 등의 모든 프로젝트 관련 정보를 포함합니다. 예를 들어, 게임 프로젝트나 웹사이트 프로젝트 등을 저장소로 만들 수 있습니다.

- `버전 관리(Version Control)`: 프로젝트의 모든 변경 내용을 추적하고 관리하는 기능입니다. 버전 관리를 통해 개발자는 프로젝트의 이전 버전을 복원하거나 수정사항을 추적할 수 있습니다. 이를 통해 협업을 원활하게 할 수 있습니다.

- `커밋(Commit)`: 프로젝트의 변경 사항을 저장소에 영구적으로 기록하는 작업입니다. 개발자는 작업을 완료한 후 변경된 파일을 커밋하여 해당 버전의 스냅샷을 생성합니다. 커밋에는 변경 내용에 대한 설명을 작성하는 것이 일반적입니다.

- `푸쉬(Push)`: 푸쉬는 개발자가 자신의 로컬 컴퓨터에서 작업한 코드 변경 내용을 원격 저장소로 업로드하는 작업을 말합니다. 푸쉬를 통해 개발자는 로컬에서 작업한 최신 코드를 원격 저장소에 공유하고, 푸쉬가 완료되면 변경된 코드가 원격 저장소에 저장되어 다른 개발자들이 직접 확인하고 사용할 수 있습니다.

- `풀(Pull)`: 풀은 개발자가 원격 저장소에 있는 데이터를 로컬 컴퓨터로 가져오는 작업을 말합니다. 풀을 통해 개발자는 Github에 업로드된 최신 버전의 내용을 로컬로 동기화하여 작업할 수 있습니다. 다른 개발자들이 원격 저장소에 푸쉬한 변경 내용을 가져와서 로컬 작업 환경을 최신 상태로 유지할 수 있습니다.

- `브랜치(Branch)`: 프로젝트의 특정 부분에 대해 독립적으로 작업할 수 있는 복사본입니다. 브랜치를 사용하면 여러 개발자가 동시에 다양한 기능을 개발하거나 버그를 수정할 수 있습니다. 개발이 완료되면 브랜치를 다시 합칠 수 있습니다.

- `풀 리퀘스트(Pull Request)`: 개발자가 자신의 작업 내용을 저장소의 다른 브랜치에 반영해달라고 요청하는 기능입니다. 다른 개발자들은 변경 내용을 검토하고 논의한 후, 풀 리퀘스트를 승인하거나 수정 사항을 요청할 수 있습니다.

- `병합(Merge)`: 브랜치에 작업한 내용을 다른 브랜치나 기본 브랜치로 통합하는 과정입니다. 풀 리퀘스트가 승인되면 변경 사항이 기본 브랜치로 병합됩니다.

- `이슈(Issue)`: 프로젝트에서 해결해야 할 작업, 버그, 기능 요청 등을 추적하는 기능입니다. 이슈는 개발자들이 프로젝트의 문제를 공유하고 협력하여 해결하는 데 사용됩니다.

---

---

# **Git Branches 관리 전략**
## **Gitflow**
### Gitflow는 Git을 기반으로 한 효율적인 브랜치 관리 전략중 하나입니다.

**Gitflow의 주요 브랜치**<br>
- Main Branch: 주요 브랜치로서, 안정된 소프트웨어 버전을 관리하는 데 사용됩니다. 보통 "master" 또는 "main"이라는 이름으로 사용됩니다.
- Develop Branch: 개발 브랜치로서, 다음 배포 버전을 준비하는 데 사용됩니다. 기능 개발이나 버그 수정과 같은 작업은 이 브랜치에서 이루어집니다.
- Feature Branch: 새로운 기능을 개발하기 위한 브랜치입니다. Develop 브랜치에서 분기하고 개발이 완료되면 Develop 브랜치로 병합합니다.
- Release Branch: 배포를 준비하기 위한 브랜치입니다. Develop 브랜치의 기능을 안정화하고 버그 수정 및 준비 작업을 수행한 후 Main 브랜치로 병합합니다.
- Hotfix Branch: 긴급한 버그 수정을 위한 브랜치입니다. Main 브랜치에서 분기하고 수정이 완료되면 Main 및 Develop 브랜치로 병합합니다.

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
