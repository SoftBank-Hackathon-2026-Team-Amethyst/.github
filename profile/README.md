# 🎉 **SoftBank Hackathon 2026**

> **원터치로, 규칙대로, 어디에나 배포한다**

금융권처럼 규제가 있는 곳에는 멀티클라우드와 **출구전략**이 필요하지만, 매번 사람이 인프라를 설계하기는 어렵습니다.<br>
저희는 필수 검사를 **기본 템플릿**으로 먼저 깔아 두고, 그 위에서 **AI 에이전트가 배포를 준비하는 플랫폼**을 만들었습니다.

<br>

---

# 💜 Team Amethyst

<div align="center">
  <img width="480" alt="원터치 배포 버튼을 누르는 토끼" src="https://raw.githubusercontent.com/SoftBank-Hackathon-2026-Team-Amethyst/one-tatchi-platform/main/docs/assets/one-touch-deploy.png" />
</div>

<br>

<table align="center">
  <tr>
    <td align="center"><img width="120" src="https://github.com/silano08.png" /></td>
    <td align="center"><img width="120" src="https://github.com/soulee-dev.png" /></td>
    <td align="center"><img width="120" src="https://github.com/hyeongrae-kim.png" /></td>
    <td align="center"><img width="120" src="https://github.com/baejun10.png" /></td>
    <td align="center"><img width="120" src="https://github.com/baekyutae.png" /></td>
  </tr>
  <tr>
    <td align="center"><b>원가연</b><br><sub><a href="https://github.com/silano08">@silano08</a></sub><br><sub>플랫폼 코어</sub></td>
    <td align="center"><b>이소울</b><br><sub><a href="https://github.com/soulee-dev">@soulee-dev</a></sub><br><sub>파이프라인</sub></td>
    <td align="center"><b>김형래</b><br><sub><a href="https://github.com/hyeongrae-kim">@hyeongrae-kim</a></sub><br><sub>에이전트 스킬</sub></td>
    <td align="center"><b>배준범</b><br><sub><a href="https://github.com/baejun10">@baejun10</a></sub><br><sub>데모 앱</sub></td>
    <td align="center"><b>배규태</b><br><sub><a href="https://github.com/baekyutae">@baekyutae</a></sub><br><sub>AI 판단 · 리포트</sub></td>
  </tr>
</table>

<br>

---

# 🐰 완땃찌(원터치) 배포
> 로컬에서 만든 웹앱을 AI 에이전트가 분석하고, 컴플라이언스 검사를 통과한 변경만 **AWS · GCP · 온프레미스**에 배포합니다.

### 👨‍💻 For Developers — *One Touch*
- `/janto-deploy` 한 번으로 **질문 → 분석 → 배포 파일 생성 → PR**까지
- `/yolo-deploy`로 리뷰 없이 테스트 환경까지. 검사가 실패하면 **AI가 최대 3회 고쳐서** 다시 올림
- 배포 결과를 **Slack**으로 받고, 버튼으로 승격 · 롤백

<br>

### 🏦 For Regulated Orgs — *Guardrails & Exit Strategy*
- 정적분석 · 테스트 · 취약점 · 시크릿 · IaC 검사를 **기본 템플릿**으로 강제. AI는 변수만 채우고 본문은 못 고침
- 같은 기능 계약 위에 **AWS · GCP · 온프레미스** 구현체를 두어 벤더를 바꿔도 앱은 그대로
- **Blue-Green** 테스트 배포 → AI 승격 판단 → 규제 대상이면 운영 앞에서 **사람 승인**

<br>

---

# 🧰 Core Tech Stack

### 🤖 Agent
<div>
  <img src="https://img.shields.io/badge/Claude%20Code-D97757?style=for-the-badge&logo=claude&logoColor=white"/>
  <img src="https://img.shields.io/badge/Agent%20Skills-8E44AD?style=for-the-badge"/>
</div>

### 🏗️ Infrastructure
<div>
  <img src="https://img.shields.io/badge/Terraform-7B42BC?style=for-the-badge&logo=terraform&logoColor=white"/>
  <img src="https://img.shields.io/badge/Amazon%20EKS-FF9900?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Google%20Cloud-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white"/>
  <img src="https://img.shields.io/badge/k3d%20(On--Prem)-FFC61C?style=for-the-badge&logo=k3s&logoColor=black"/>
</div>

### 🚀 Delivery
<div>
  <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white"/>
  <img src="https://img.shields.io/badge/Helm-0F1689?style=for-the-badge&logo=helm&logoColor=white"/>
  <img src="https://img.shields.io/badge/Argo%20Rollouts-EF7B4D?style=for-the-badge&logo=argo&logoColor=white"/>
</div>

### 🛡️ Checks & Observability
<div>
  <img src="https://img.shields.io/badge/Trivy-1904DA?style=for-the-badge&logo=trivy&logoColor=white"/>
  <img src="https://img.shields.io/badge/Gitleaks-DC3545?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white"/>
  <img src="https://img.shields.io/badge/Slack%20Bolt-4A154B?style=for-the-badge&logo=slack&logoColor=white"/>
</div>

<br>

---

# 📂 Repository Structure

| 저장소 | 설명 |
|---|---|
| **[one-tatchi-platform](https://github.com/SoftBank-Hackathon-2026-Team-Amethyst/one-tatchi-platform)** | 기본 템플릿. Terraform 모듈(AWS · GCP · 온프레미스), App Chart, 재사용 워크플로, 에이전트 스킬, Slack 봇 |
| **[demo-app](https://github.com/SoftBank-Hackathon-2026-Team-Amethyst/demo-app)** | 배포 대상 데모 앱(Vite React + Fastify + PostgreSQL). 템플릿을 태그로 참조만 합니다 |
