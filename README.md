# test



MinIO(R) 기반 Bitnami 개체 스토리지
MinIO(R)는 주로 구조화되지 않은 데이터(예: 사진, 비디오, 로그 파일 등)를 저장하는 데 사용되는 Amazon S3 클라우드 스토리지 서비스와 호환되는 개체 스토리지 서버입니다.

MinIO® 기반 Bitnami Object Storage 개요

면책 조항: 모든 소프트웨어 제품, 프로젝트 및 회사 이름은 해당 소유자의 상표(TM) 또는 등록(R) 상표이며 이들의 사용이 제휴 또는 보증을 의미하지 않습니다. 이 소프트웨어는 하나 이상의 오픈 소스 라이센스에 따라 귀하에게 라이센스가 부여되며 VMware는 소프트웨어를 있는 그대로 제공합니다. MinIO(R)는 미국 및 기타 국가에서 MinIO Inc.의 등록 상표입니다. Bitnami는 MinIO Inc.와 제휴, 연결, 승인, 보증 또는 어떠한 방식으로도 공식적으로 연결되어 있지 않습니다. MinIO(R)는 GNU AGPL v3.0에 따라 라이선스가 부여됩니다.

TL;DR
helm install my-release oci://registry-1.docker.io/bitnamicharts/minio
소개
이 차트는 Helm 패키지 관리자를 사용하여 Kubernetes 클러스터 에서 MinIO® 배포를 부트스트랩합니다 .

클러스터에서 Helm 차트의 배포 및 관리를 위해 Bitnami 차트를 Kubeapps 와 함께 사용할 수 있습니다 .

MinIOreg 기반 Bitnami Object Storage를 사용하려고 합니다. 생산 중? Bitnami 애플리케이션 카탈로그의 엔터프라이즈 버전인 VMware 애플리케이션 카탈로그를 사용해 보십시오 .

전제 조건
쿠버네티스 1.19+
투구 3.2.0+
기본 인프라에서 PV 제공자 지원
차트 설치
릴리스 이름으로 차트를 설치하려면 다음을 수행하십시오 my-release.

helm install my-release oci://registry-1.docker.io/bitnamicharts/minio
이러한 명령은 기본 구성의 Kubernetes 클러스터에 MinIO®를 배포합니다. 매개 변수 섹션에는 설치 중에 구성할 수 있는 매개변수가 나열됩니다.

팁 : 다음을 사용하여 모든 릴리스를 나열하십시오.helm list
