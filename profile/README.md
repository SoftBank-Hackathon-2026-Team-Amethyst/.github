<p align="center">
  <img src="https://raw.githubusercontent.com/SoftBank-Hackathon-2026-Team-Amethyst/one-tatchi-platform/main/docs/assets/one-touch-deploy.png" alt="원터치 배포 버튼을 누르는 토끼" width="480">
</p>

<h1 align="center">💜 Team Amethyst · 완땃찌(원터치) 배포</h1>

<p align="center">
  <b>로컬에서 만든 웹앱을 AI 에이전트가 분석하고,<br>컴플라이언스 검사를 통과한 변경만 AWS · GCP · 온프레미스에 배포합니다.</b>
</p>

<p align="center">
  <img alt="SoftBank Hackathon 2026" src="https://img.shields.io/badge/SoftBank_Hackathon-2026-8E44AD?style=flat-square">
  <img alt="Claude Code" src="https://img.shields.io/badge/Agent-Claude_Code-D97757?style=flat-square">
  <img alt="Terraform" src="https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white">
  <img alt="Helm" src="https://img.shields.io/badge/Helm-0F1689?style=flat-square&logo=helm&logoColor=white">
  <img alt="GitHub Actions" src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white">
</p>

---

## 🐰 무엇을 하나요

금융권처럼 규제가 있는 곳에는 멀티클라우드와 **출구전략**이 필요하지만, 매번 사람이 설계하기는 어렵습니다.
그래서 정적분석 · 테스트 · 취약점 검사 같은 필수 항목을 **기본 템플릿**으로 먼저 깔아 두고,
AI 에이전트는 서비스를 분석해 **변수만 채우고**, 배포 파이프라인이 규칙대로 반영합니다.

| 경로 | 흐름 |
|---|---|
| `/janto-deploy` (정석) | 질문 → 분석 → 배포 파일 생성 → `main` PR → 사람 리뷰 → 테스트 → 운영 |
| `/yolo-deploy` (예외) | 리뷰 없이 테스트 환경까지. 검사가 실패하면 AI가 최대 3회 고쳐서 다시 올림 |

배포는 Blue-Green으로 테스트에 먼저 올라가고, AI가 승격 여부를 판단합니다. 규제 대상이면 운영 앞에서 사람이 승인합니다.

## 📦 Repositories

| 레포 | 설명 |
|---|---|
| [**one-tatchi-platform**](https://github.com/SoftBank-Hackathon-2026-Team-Amethyst/one-tatchi-platform) | 기본 템플릿: Terraform 모듈(AWS · GCP · 온프레미스), App Chart, 재사용 워크플로, 에이전트 스킬, Slack 봇 |
| [**demo-app**](https://github.com/SoftBank-Hackathon-2026-Team-Amethyst/demo-app) | 배포 대상 데모 앱 (Vite React + Fastify + PostgreSQL). 템플릿을 태그로 참조만 함 |

## 👥 Team

<table>
  <tr>
    <td align="center"><a href="https://github.com/silano08"><img src="https://github.com/silano08.png" width="80"><br><b>원가연</b></a><br>플랫폼 코어</td>
    <td align="center"><a href="https://github.com/soulee-dev"><img src="https://github.com/soulee-dev.png" width="80"><br><b>이소울</b></a><br>파이프라인</td>
    <td align="center"><a href="https://github.com/hyeongrae-kim"><img src="https://github.com/hyeongrae-kim.png" width="80"><br><b>김형래</b></a><br>에이전트 스킬</td>
    <td align="center"><a href="https://github.com/baejun10"><img src="https://github.com/baejun10.png" width="80"><br><b>배준범</b></a><br>데모 앱</td>
    <td align="center"><a href="https://github.com/baekyutae"><img src="https://github.com/baekyutae.png" width="80"><br><b>배규태</b></a><br>AI 판단 · 리포트</td>
  </tr>
</table>
