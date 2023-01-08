# 2021 오픈소스 컨트리뷰션 아카데미
2021 오픈소스 컨트리뷰션 아카데미에 참여하며 했던 기여를 정리한 글입니다.     
## 목차
* [참여했던 프로젝트](https://github.com/yujung7768903/contribution-academy-2021/blob/main/README.md#%EC%B0%B8%EC%97%AC%ED%96%88%EB%8D%98-%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8)
* [Masters 기간에 했던 기여 (2022.09 ~ 2022.11)](https://github.com/yujung7768903/contribution-academy-2021/blob/main/README.md#masters-%EA%B8%B0%EA%B0%84%EC%97%90-%ED%96%88%EB%8D%98-%EA%B8%B0%EC%97%AC-202209--202211)
* [연계 인턴십 기간에 했던 기여 (2022.11 ~ 2022.12)](https://github.com/yujung7768903/contribution-academy-2021/blob/main/README.md#%EC%97%B0%EA%B3%84-%EC%9D%B8%ED%84%B4%EC%8B%AD-%EA%B8%B0%EA%B0%84%EC%97%90-%ED%96%88%EB%8D%98-%EA%B8%B0%EC%97%AC-202211--202212)
* [배운점 & 느낀점](https://github.com/yujung7768903/contribution-academy-2021/blob/main/README.md#%EC%97%B0%EA%B3%84-%EC%9D%B8%ED%84%B4%EC%8B%AD-%EA%B8%B0%EA%B0%84%EC%97%90-%ED%96%88%EB%8D%98-%EA%B8%B0%EC%97%AC-202211--202212)

## 참여했던 프로젝트
**Backend.AI - 래블업에서 개발한 Backend.AI는 GPU 특화 머신러닝 연산자원 관리 플랫폼**    

<img height="350" alt="Screen Shot 2023-01-08 at 3 25 17 PM" src="https://user-images.githubusercontent.com/68562176/211183482-1b38c2ef-41b5-4783-920f-59b9084789c7.png"> <img height="350" alt="Screen Shot 2023-01-08 at 3 25 45 PM" src="https://user-images.githubusercontent.com/68562176/211183502-7b5d1df9-074f-4708-8ef0-0678eed072d2.png">

* 실행 환경을 선택하고 자원을 원하는만큼 할당하여 세션을 만들 수 있습니다. 해당 세션에서 복잡한 개발환경 세팅없이 원하는 환경에서 개발할 수 있습니다.
<img width="900" alt="Screen Shot 2023-01-08 at 3 29 03 PM" src="https://user-images.githubusercontent.com/68562176/211183597-fffaeec3-77a2-4953-a6d9-4cad0af6b0e4.png">

* 할당된 자원과 사용량 확인이 가능합니다.

## Masters 기간에 했던 기여 (2022.09 ~ 2022.11)
➡️ [2021 오픈소스 컨트리뷰션 아카데미 회고 글 보러가기](https://velog.io/@youjung/2021-%EC%98%A4%ED%94%88%EC%86%8C%EC%8A%A4-%EC%BB%A8%ED%8A%B8%EB%A6%AC%EB%B7%B0%EC%85%98-%EC%95%84%EC%B9%B4%EB%8D%B0%EB%AF%B8-%ED%9B%84%EA%B8%B0)    
### [Front-end]
#### 1. UI Bug관련 이슈 생성 및 해결     
윈도우의 너비가 넓어지면 세션 메뉴에서 자원 사용량과 세션 리스트 패널의 너비가 달라지는 것을 발견하고, 통일시키는 방향이 보기 더 좋을 것이라 판단하여 이슈를 생성하고 해결했습니다. 이 이슈를 통해서 width가 auto일 때 display에 따라 어떻게 너비가 결정되는지에 대해 알게 되었습니다.
* 생성한 Issue: https://github.com/lablup/backend.ai-webui/issues/1113
* PR(Merged): https://github.com/lablup/backend.ai-webui/pull/1117

#### 2. 여백을 통일시키는 이슈 진행      
각 페이지별로 여백의 크기가 달라서 통일시키는 이슈를 진행했습니다. 이 이슈를 통해서 마진 상쇄에 대해 배울 수 있었습니다.
* PR(Merged): https://github.com/lablup/backend.ai-webui/pull/1118

#### 3. 중복 스크롤 제거
약관 창에 스크롤이 불필요하게 2개가 존재하는 걸 발견했습니다. 내리는 동작이 부자연스럽고 하나만 있어도 될 것 같아서 이슈를 생성하고 해결했습니다.
* PR(Merged): https://github.com/lablup/backend.ai-webui/pull/1142

## 연계 인턴십 기간에 했던 기여 (2022.11 ~ 2022.12)
➡️ [오픈소스 컨트리뷰션 아카데미 연계 인턴십 회고 글 보러가기](https://velog.io/@youjung/IT-%EC%8A%A4%ED%83%80%ED%8A%B8%EC%97%85%EC%97%90%EC%84%9C-%EA%B2%BD%ED%97%98%ED%95%9C-%EC%B2%AB-%EC%9D%B8%ED%84%B4%EC%8B%AD-%EB%9E%98%EB%B8%94%EC%97%85)

### [Front-end]
#### 1. Backend.AI의 WebUI 컴포넌트와 관련된 bug해결
회원가입 약관 창 종료 후 다시 오픈이 되지 않는 문제를 해결했습니다. 변수 재할당이 이뤄지지 않아 발생한 문제로 자식 컴포넌트가 닫힐 때 이벤트를 발생시켜 부모 컴포넌트에서 처리하도록 진행했습니다.
* PR(Merged): https://github.com/lablup/backend.ai-webui/pull/1160

#### 2. session 페이지의 session list와 관련된 bug 해결
테이블 셀 안에 있는 2개의 아이템이 겹치는 문제를 해결했습니다. 처음에는 아이템이 겹치니까 단순하게 너비를 늘려서 해결하려 했습니다. 하지만 그 과정에서 문제가 발생하여 사용자의 입장에서 바라보며 어떤 방법으로 해결하는 것이 좋을지 고민하는 시간을가졌습니다.
* PR(Merged): https://github.com/lablup/backend.ai-webui/pull/1170

### [Back-end]
#### 1. Backend.AI의 manager 명령어 추가하기
Click 패키지를 사용하여 데이터베이스에 쌓이는 데이터를 삭제하고, 디스트 공간을 확보하는 명령어를 만들었습니다. 디스크 공간 확보를 위한 PostgreSQL VACUUM 작업이 수행될 때 발생한 에러를 해결하면서 CREATE DATABASE나 VACUUM과 같은 명령어들을 트랜잭션 안에서 실행이 불가하기 때문에, AUTOCOMMIT 모드로 바꿔주어야한다는 것을 알게 되었습니다.
* PR(Merged): https://github.com/lablup/backend.ai-manager/pull/498

#### 2. Backend.AI의 manager 컴포넌트에서 조건 검사와 관련된 이슈 진행
세션 생성 조건을 검사하는 위치를 변경하여 큐에서 대기할 필요없이 바로 검사를 수행할 수 있도록 개선 작업을 했습니다. 이 이슈를 통해 조건을 검사하는 것 뿐만 아니라 언제 하는지도 성능 향상을 위해 중요하다는 것을 알게 되었습니다.
* PR(Merged): https://github.com/lablup/backend.ai-manager/pull/504

#### 4. 데이터베이스 agents 테이블의 자원그룹을 변경하는 기능 추가
자원그룹 옵션을 변경 기능 추가를 위해 Toml 설정파일 값과 데이터베이스의 값을 모두 변경시키는 메서드를 추가하였습니다. Manager 컴포넌트가 클라이언트로부터 요청을 받으면 Toml 설정 파일의 값을 변경하기 위해 Agent라는 컴포넌트에서 작업이 필요했기 때문에 Agent에 RPC 메서드를 추가하고 Manager에서는 요청하는 방식으로 진행했습니다. 
* Manager PR(Merged): https://github.com/lablup/backend.ai-manager/pull/511
* Agent PR(Merged): https://github.com/lablup/backend.ai-agent/pull/327

## 배운점 & 느낀점
* 다른 사람이 짠 코드를 분석하고 이해하는 것에 익숙해졌습니다. 그래서 행사 이후 참여한 프로젝트에서는 구조, 코드 스타일, 선호하는 변수 네이밍 방식에 대해 파악하고 작업할 수 있었습니다. 또한 코드를 통해 습득하는 것이 많아졌다고 생각합니다.
* Issue를 통해 할 일을 관리하고, Fork한 후 작업하고, Pull Request를 통해 코드 병합을 요청하는 Github 협업 방식을 익혔습니다. Git 명령어에 능숙해지고, 모르는 명령어도 검색을 통해 어려움 없이 사용할 수 있게 되었습니다.
* 문제가 생겼을 때 빠르게 해결하는 것도 중요하지만, 특히 UI와 관련해서는 사용자의 입장에서 바라보면서 다양한 해결 방법을 고민해보는 것이 중요하다는 것을 깨달았습니다.
