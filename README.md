# AWS 기반 Infra 구축
     AWS 기반 Infra 구축
     WEB-WAS-DB를 연동하여, 3-Tier 웹 서비스 운영
     WEB-WAS 분리
     Tomcat의 Error Page 구현
     Prometheus, Grafana를 활용해 Resources Monitoring 구축
     CloudWatch를 활용해 Application Monitoring 구축
     SNS를 통한 Application Error 메일 알림 구현
     Slack 통한 각 서비스 알람 구현
## 진행 기간
- 2022.08.29 ~ 2022.09.16

</br>

## 팀 구성
- Infra 구축 5명

</br>

## 사용 기술
#### CSP
<img src="https://img.shields.io/badge/Amazon AWS-232F3E?style=flat-square&logo=Amazon AWS&logoColor=white"> <!--AWS-->
#### OS
<img src="https://img.shields.io/badge/Amazon Linux-232F3E?style=flat-square&logo=Amazon AWS&logoColor=white"> <!--amazon linux-->
#### Database
<img src="https://img.shields.io/badge/mysql-4479A1?style=flat-square&logo=mysql&logoColor=white"> <!--Mysql-->
#### Monitoring
<img src="https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=Prometheus&logoColor=white"> <!--Prometheus--> 
<img src="https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=Grafana&logoColor=white"> <!--Grafana--> 
#### Framework
<img src="https://img.shields.io/badge/Spring-6DB33F?style=flat-square&logo=Spring&logoColor=white"> <!--Spring-->
#### Team Collabolation Tool
<img src="https://img.shields.io/badge/Notion-000000?style=flat-square&logo=Notion&logoColor=white"> <!--Notion-->
<img src="https://img.shields.io/badge/Drawio-000000?style=flat-square&logo=Drawio&logoColor=white"> <!--Draw.io-->

</br>

## 담당한 업무
- AWS Infra 구축
    - IAM, VPC, EC2, RDS, EFS, ALB, NLB, AS, ACM, Route53, CDN, CloudWatch, SNS
- EFS 구축
    - WEB/WAS Resoures의 저장과 관리
    - WEB/WAS Resoures를 각각 독립된 EFS로 관리
- WEB/WAS를 분리
    - 정적인 컨텐츠는 WEB에서 처리
    - 동적인 컨텐츠는 WAS에서 처리
- WAS의 Error Page를 구현
    - Tomcat Server가 down 될 시, 담당자 연락처가 나오도록 설정
- CloudFront 구축
    - 정적 및 동적 웹 컨텐츠를 고객에게 더 빠르게 배포
- Route53과 ACM 구축
    - 고객들이 쉽고 빠르게 웹 서비스를 이용
    - HTTPS Protocol를 사용하여 보안을 강화

</br>

## 상세 내용 
### 고객 요구사항
![image](https://user-images.githubusercontent.com/110655823/215494913-a04785ef-69bf-483b-a977-4ba859f66757.png)
>- 고가용성, 실시간 모니터링, Error Page를 구성하여 프로젝트 진행
### Infra Architecture
![image](https://user-images.githubusercontent.com/110655823/215495265-30c7cdd6-5be8-4d70-b560-f72a45b5dddc.png)
>- 관리자는 bastion을 통해 웹 서비스를 운영 및 관리
>- 고객은 route53에 등록된 도메인을 통해 웹 서비스 이용
>- EFS를 사용하여 WEB/WAS 리소스들의 저장과 관리
>- Application Monitoring은 CloudWatch로 로그를 수집 및 필터링 → Error 발생 시 SNS을 통해 메일 알림
>- Resources Monitoring은 Node-Exporter로 메트릭 정보를 수집 → Prometheus TSDB로 전달 → Grafana를 통해 수집된 매트릭을 시각화

### Security Group
![image](https://user-images.githubusercontent.com/110655823/215495468-ceb8bf50-58d9-4b1e-b9ec-9efeb5cb34fa.png)

### - [내부 인프라](https://github.com/hyunjaebok/AWeSome_AWS_3Tier_SemiProject/tree/main/내부%20인프라)
### - [외부 인프라](https://github.com/hyunjaebok/AWeSome_AWS_3Tier_SemiProject/tree/main/외부%20인프라)


</br>

## 구축 과정
### - Notion Link(https://www.notion.so/AWS-Infra-8a62fe0dcd8c488fbb6655e0f5f624b3)

</br>

---

### [👈 Go back 👈](https://github.com/hyunjaebok)
