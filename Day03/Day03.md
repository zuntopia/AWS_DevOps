> https://12factor.net/ko/

# Test of DevOps
* 사람이 하지마라
* 품질은 기계가 보증한다

### 테스트 단계
* 유닛테스트 -> 서비스/통합/구성 테스트 -> 성능/규정테스트 -> UI 테스트

### 프로덕션 복제
* 프로덕션 레벨과 최대한 동일하게 구성을 해야 한다.
* mocking 서버 구성

### CI / CD 각 단계에서 테스트 진행해야 함
* CI: 개발: uni test / static analist
* CI: Build: 통합 / 구성 / 회귀
* CD: 스테이징: 시스템, 성능, 로드, 규정 준수, UAT
* CD: 프로덕션: A/B, 카나리아

# 성능 테스트

# 성능 기준선

# cloudwatch logs

### insight

# BP
* AMI / CloudTemplate 사용
* CI 적용
* AWS API로 반복테스트

# OpsWorks
* Chef / puppet

# 로그수집
* 람다가 중요하다
* 로그 수집 중 람다 실행-> elastic domain에 저장

# AMI
### AMI 빌드전략
* skinny
* gold
* silver

# AWS System Manager
* Secret manager vs parameter store

> https://www.slideshare.net/awskr/packer-ansible-ami-autoscaling-group-88560117

* 오토스케일링 그룹 교체
  - launch configuration 을 새로 만든다


# Docker / ECS
### Container
### in AWS: ECS
### AWS Fargate
* Container 가 사용한 CPU / Memory 에 대한 비용만 지불

### workflow
* dockefile -> Elastic Container Service -> ECS -> service

### 작업 배치
* 전략: 인스턴스 종료 기준을 선택
* 제약조건: ?

### 