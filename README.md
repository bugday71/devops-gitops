# devops-gitops

## Structure
- apps/devops-app/base: 공통 매니페스트
- apps/devops-app/overlays/dev: 개발 환경 오버레이
- apps/devops-app/overlays/prod: 운영 환경 오버레이
- argocd: Argo CD Application 리소스

## Update image tag
Jenkins에서 새 태그를 푸시한 뒤, GitOps 방식으로 아래 파일의 `newTag`를 갱신하세요.
- apps/devops-app/overlays/dev/kustomization.yaml
- apps/devops-app/overlays/prod/kustomization.yaml
