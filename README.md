<div align="center">

# 함경재 &nbsp;·&nbsp; Gyungjae Ham

**Backend Engineer**

응답 지연과 외부 시스템 의존처럼 구조에서 비롯되는 문제를<br/>
비동기 처리 · 배치 · 사전 적재로 풀어내는 5년차 백엔드 엔지니어입니다.

<p>
  <a href="mailto:gyeongjae.h.dev@gmail.com">
    <img src="https://img.shields.io/badge/Email-gyeongjae.h.dev@gmail.com-0F172A?style=flat-square&logo=gmail&logoColor=white" alt="Email" />
  </a>
  <a href="https://github.com/gyungjae-ham">
    <img src="https://img.shields.io/badge/GitHub-gyungjae--ham-0F172A?style=flat-square&logo=github&logoColor=white" alt="GitHub" />
  </a>
  <a href="https://gyungjae-ham.github.io">
    <img src="https://img.shields.io/badge/Blog-gyungjae--ham.github.io-0F172A?style=flat-square&logo=githubpages&logoColor=white" alt="Blog" />
  </a>
</p>

</div>

<br/>

## 핵심 성과

| 무엇을 했나 | 결과 |
| --- | --- |
| 외부 API 실시간 호출을 30분 단위 배치 사전 적재로 재설계 | **42초 → 20ms** |
| 대용량 주문 처리 파이프라인 재구성 (N+1 제거 · BatchInsert) | **60초 → 3~5초** |
| Slow Query 진단 · 페이지네이션으로 주요 API 튜닝 | **1,200ms → 55ms** |
| 테스트 병렬 실행 전환으로 CI 파이프라인 최적화 | **3분 20초 → 21초** |
| K6 부하 테스트 기반 Pod 리소스 재배분 | **피크 timeout 0건** |

> 공통점은 하나입니다 — 외부 의존과 동기 처리에서 오는 병목을, **구조를 바꿔** 제거했습니다.

<br/>

## 지금 하는 일

**BIND** 에서 미디어 수집·변환 파이프라인과 인증 백엔드를 맡고 있습니다.

- 인스타그램 게시물 **자동 수집 파이프라인** — Redis 분산락으로 중복 차단, S3 스트리밍 업로드(8MB 청크). 수동 등록 0건, 노출 지연 `1~2일 → 24시간 이내`
- **HLS 영상 변환 파이프라인** — MediaConvert 대신 ffmpeg + Celery로 직접 구축, 6초 segment 분할로 모바일 점진 재생
- **전화번호 인증 백엔드 이관** — 검증을 서버로 옮기고 Redis 레이트리밋(시간당 10회), 테스트 213개로 클라이언트 우회 경로 제거

<br/>

## 기술 스택

| | |
| --- | --- |
| **주력** | ![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white) ![Java](https://img.shields.io/badge/Java-0F172A?style=flat-square&logo=openjdk&logoColor=white) ![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white) ![JPA](https://img.shields.io/badge/JPA_·_Querydsl-59666C?style=flat-square&logo=hibernate&logoColor=white) |
| **병행** | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![Django](https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white) ![Celery](https://img.shields.io/badge/Celery-37814A?style=flat-square&logo=celery&logoColor=white) ![Spring Batch](https://img.shields.io/badge/Spring_Batch-6DB33F?style=flat-square&logo=spring&logoColor=white) |
| **데이터** | ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white) |
| **인프라** | ![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white) ![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white) ![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white) ![K6](https://img.shields.io/badge/K6-7D64FF?style=flat-square&logo=k6&logoColor=white) |

<br/>

## 경력

`BIND` 2026.01 ~ 재직 중 &nbsp;·&nbsp; `위밋모빌리티` 2024.10 ~ 2026.01 &nbsp;·&nbsp; `라이너스` 2023.07 ~ 2024.09 &nbsp;·&nbsp; `그 외` 레인보우8 · 쿠돈

<sub>전남대학교 경제학과 학사 · 총 경력 5년 1개월</sub>
