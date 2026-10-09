# 🎉 **SoftBank Hackathon 2026**

> **원터치로, 규칙대로, 어디에나 배포한다**

개발자는 인프라와 배포 파이프라인까지 세세하게 신경 쓰고 싶지 않습니다. **AI에게 맡기고, 원터치!** 🐰<br>
하지만 현실은 그렇게 녹록지 않습니다. 원터치는 보통 많은 **보안의 희생**을 요구하니까요.

**그렇다면, 어떻게 해야 안전하게 원터치할 수 있을까요?**

저희의 답은 **"AI는 변수만 채우고, 규칙은 템플릿이 지킨다"** 입니다.<br>
정적분석 · 테스트 · 취약점 검사를 **기본 템플릿**으로 먼저 깔아 두고, AI 에이전트는 그 위에서 배포를 준비합니다.<br>
템플릿은 AWS · GCP · 온프레미스를 같은 방식으로 다뤄서, 클라우드를 옮겨야 할 때를 위한 **출구전략**도 함께 갖춥니다.

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

### 👩‍💻 For Product Engineers — *One Touch*
> 인프라는 몰라도 된다. 앱만 만들면 된다.

| 지금까지는 | 원터치로는 |
|---|---|
| Dockerfile · Helm · Terraform · CI를 직접 짜거나 플랫폼 팀에 요청하고 기다림 | `/janto-deploy` 한 번에 **질문 → 분석 → 배포 파일 생성 → PR** |
| 검사가 왜 떨어졌는지 로그를 뒤지며 고침 | `/yolo-deploy`면 **AI가 원인을 고쳐 최대 3회** 다시 올림 |
| 승격 · 롤백하려고 콘솔이나 kubectl을 열어야 함 | **Slack 버튼**으로 승격 · 취소 · 되돌리기 |

<br>

### 🛡️ For Platform Engineers (DevSecOps) — *Guardrails & Exit Strategy*
> 팀마다 따로 리뷰하지 않아도 된다. 규칙은 템플릿이 지킨다.

| 지금까지는 | 원터치로는 |
|---|---|
| 팀마다 다른 배포 파일을 하나하나 리뷰하고, 검사 단계가 빠졌는지 확인 | 정적분석 · 테스트 · 취약점 · 시크릿 · IaC 검사가 **기본 템플릿에 고정**. AI는 변수만 채우고 본문은 못 고침 |
| 클라우드를 옮기려면 인프라 코드를 처음부터 다시 작성 | 같은 기능 계약 위에 **AWS · GCP · 온프레미스** 구현체. 대상만 바꾸면 앱은 그대로 (**출구전략**) |
| 템플릿을 고치면 모든 레포에 직접 반영 요청 | 새 태그를 내면 각 레포에 **버전 올리기 PR이 자동으로** 열림 |
| 운영 배포마다 사람이 지켜봄 | **Blue-Green** 테스트 배포 → AI 승격 판단, 규제 대상만 운영 앞에서 **사람 승인** |

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
