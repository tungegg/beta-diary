# Beta Diary AWS 네트워크 설계

## 목표
Spring Boot 애플리케이션을 AWS에서 서비스하기 위한 네트워크 설계

## 네트워크 구성
- VPC: 10.20.0.0/16
- Public Subnet: 10.20.1.0/24
- Private Subnet: 10.20.2.0/24
- Internet Gateway: 외부 인터넷 연결
- Route Table: 서브넷별 라우팅 관리
- Security Group: EC2 접근 제어

## 검토할 사항
- EC2를 Public Subnet에 배치하는 이유
- 외부 사용자가 EC2에 접근하는 경로
- HTTPS 443 포트 허용 정책
- 도메인 및 SSL/TLS 인증서 적용 방법

## 현재 상태
네트워크 아키텍처 설계 중. 실제 AWS 리소스 미배포.
