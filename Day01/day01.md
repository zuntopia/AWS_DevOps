# 데브옵스의 이점
* 지속적 통합
* 지속적 전달
* 마이크로서비스
* 코드형 인프라
* 모니터링 및 로깅
* 소통 및 협업

# 지속적 통합
* 변경사항을 정기적으로 병합 / 빌드 / 테스트 수행

# 지속적 전달
1. 개발자: 마스터로 커밋
2. CI 서버: clone / build /test 수행
3. CI 서버: artifact build
4. package build
5. 패키지 저장

# (참고) Code Review
1. 가독성
2. 테스트코드가 이 코드의 작동을 보장하는지

#
aws iam create-user ...

# DevSecOps
* 보안도 오너십을 갖는다
* 보안 / 안정성은 타협하는 기준이 아님
* 자동화 필요
* CI/CD의 연장선 / 파이프라인 전체에서 매번 검사 수행

### AWS - IAM Role
* 로그인 방법
  * ID / Password
  * Role
    * 장기자격증명 지정
    * 교차게정 지원
    * API 에 대한 조건부 access 제공

### 보안 방식
* CI / CD 파이프라인 보관
  * 역할기반 접근
* CI / CD 파이프라인 내에서 보관
* 인프라 자동화

### AWS 에서 사용
* AWS CodeCommit - AWS CodeBuild - AWS CodeDeploy - AWS CloudWatch  
  ㄴ AWS CodePipeline - AWS Cloudformation - AWS Config  

### 보안자동화
* CloudFormation
  * 소유권 분리
* 규정 준수가 중요함
* 중요 업무에서 미인가 계정 이용 방지
* 중대 이밴트는 자동대응
  * Large Scale Event

### IAM 자격증명
* QueryAPI
* SDK
* CLI
* Management Console
* 최소권한원칙
* 역할-리소스의 신뢰관계 설정

### MFA
* 로그인 외에 특정 명령 수행에서도 사용가능

### AWS 계정보안
* 로그 분리 보관