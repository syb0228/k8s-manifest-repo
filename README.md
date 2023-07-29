# Amazon EKS Demo 
This repo holds **React Frontend sample** for [Amazon EKS Hands on Lab](https://master.d3s71i2n51x60t.amplifyapp.com/ko/)
- AWS 워크샵에서 컨테이너 이미지를 만드는 것을 시작으로 Amazon EKS에 컨테이너를 배포하여 웹 페이지를 올리는 실습 진행

### 활동 내용
```
01 AWS Cloud9을 통한 실습 환경 구축
02 도커를 이용하여 컨테이너 이미지 생성
03 컨테이너 이미지를 ECR에 업로드
04 Amazon EKS 클러스터 구축 및 서비스 배포
05 AWS Fargate 사용하기
06 Container Insights 사용하기
07 Autoscaling Pod & Cluster
08 Cluster Autoscaler 적용하기
09 CI/CD for EKS cluster
```

### EKS 클러스터, Kubernetes를 위한 CI/CD
- Github에 위치한 application 소스와 k8s manifests의 변경 사항이 발생될 때마다 자동으로 Github Action을 통해서 빌드/통합(CI, Continuous Integration)함
- 통합된 배포 대상을 ArgoCD를 통해 k8s 클러스터에 배포(CD, Continuous Deployment)하는 일종의 gitops 파이프라인을 만드는 실습 진행

### CI/CD 파이프라인 구성
![image](https://github.com/syb0228/front-app-repo/assets/62875437/2902d2a6-8186-4c1d-9221-d09bc4ed6ce7)

### 완성된 CI/Cd 파이프라인의 동작 흐름
![image](https://github.com/syb0228/front-app-repo/assets/62875437/0f69140a-8c5a-49b1-82a6-49db2c77d83c)

### CI/CD 파이프라인 구성하기
- 두 개의 레파지토리 생성
```
front-app-repo : Frontend 소스가 위치한 레파지토리
k8s-manifest-repo : K8S 관련 메니페스트가 위치한 레파지토리
```

### 자세한 내용 정리
[syb0228.log - Amazon EKS로 웹 애플리케이션 구축하기](https://velog.io/@syb0228/Amazon-EKS%EB%A1%9C-%EC%9B%B9-%EC%95%A0%ED%94%8C%EB%A6%AC%EC%BC%80%EC%9D%B4%EC%85%98-%EA%B5%AC%EC%B6%95%ED%95%98%EA%B8%B0)
