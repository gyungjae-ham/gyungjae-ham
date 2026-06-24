<div align="center">

# 함경재 &nbsp;·&nbsp; Gyungjae Ham

<a href="https://github.com/gyungjae-ham">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=6366F1&center=true&vCenter=true&width=620&height=45&lines=Backend+Engineer+%C2%B7+5%2B+years;Async+%C2%B7+Batch+%C2%B7+Preloading;42s+%E2%86%92+20ms+%E3%85%A4%7C%E3%85%A4+60s+%E2%86%92+3s;%EA%B5%AC%EC%A1%B0%EB%A5%BC+%EB%B0%94%EA%BE%B8%EC%96%B4+%EB%B3%91%EB%AA%A9%EC%9D%84+%EC%97%86%EC%95%B0%EB%8B%88%EB%8B%A4" alt="typing" />
</a>

<p>
  응답 지연과 외부 시스템 의존처럼 <strong>구조에서 비롯되는 문제</strong>를<br/>
  비동기 처리 · 배치 · 사전 적재로 풀어내는 5년차 백엔드 엔지니어입니다.
</p>

<p>
  <a href="mailto:gyeongjae.h.dev@gmail.com">
    <img src="https://img.shields.io/badge/Email-6366F1?style=for-the-badge&logo=gmail&logoColor=white&labelColor=0F172A" alt="Email" />
  </a>
  <a href="https://github.com/gyungjae-ham">
    <img src="https://img.shields.io/badge/GitHub-6366F1?style=for-the-badge&logo=github&logoColor=white&labelColor=0F172A" alt="GitHub" />
  </a>
  <a href="https://gyungjae-ham.github.io">
    <img src="https://img.shields.io/badge/Blog-6366F1?style=for-the-badge&logo=githubpages&logoColor=white&labelColor=0F172A" alt="Blog" />
  </a>
</p>

</div>

<br/>

## 🚀 임팩트

<table>
<tr>
<td align="center" width="33%">
<img src="https://img.shields.io/badge/42초_→_20ms-6366F1?style=for-the-badge&labelColor=0F172A" alt="42s to 20ms" /><br/>
<sub><b>외부 API 사전 적재 재설계</b><br/>실시간 호출 → 30분 배치 조회</sub>
</td>
<td align="center" width="33%">
<img src="https://img.shields.io/badge/60초_→_3~5초-7C3AED?style=for-the-badge&labelColor=0F172A" alt="60s to 3s" /><br/>
<sub><b>대용량 주문 처리 재구성</b><br/>N+1 제거 · BatchInsert</sub>
</td>
<td align="center" width="33%">
<img src="https://img.shields.io/badge/1,200ms_→_55ms-2563EB?style=for-the-badge&labelColor=0F172A" alt="1200ms to 55ms" /><br/>
<sub><b>Slow Query 진단 · API 튜닝</b><br/>주기적 서버 다운 해결</sub>
</td>
</tr>
<tr>
<td align="center" width="33%">
<img src="https://img.shields.io/badge/3분_20초_→_21초-8B5CF6?style=for-the-badge&labelColor=0F172A" alt="CI" /><br/>
<sub><b>CI 테스트 병렬화</b><br/>700+ 테스트 실행 최적화</sub>
</td>
<td align="center" width="33%">
<img src="https://img.shields.io/badge/유실률_0%25-0EA5E9?style=for-the-badge&labelColor=0F172A" alt="0 loss" /><br/>
<sub><b>webhook 서버 분리</b><br/>출결·Zoom 데이터 무결성 확보</sub>
</td>
<td align="center" width="33%">
<img src="https://img.shields.io/badge/timeout_0건-06B6D4?style=for-the-badge&labelColor=0F172A" alt="0 timeout" /><br/>
<sub><b>K6 부하 테스트 · Pod 재배분</b><br/>피크 시간대 가용성 확보</sub>
</td>
</tr>
</table>

<div align="center">
<sub>💡 공통점은 하나 — 외부 의존과 동기 처리에서 오는 병목을, <b>구조를 바꿔</b> 제거했습니다.</sub>
</div>

<br/>

## 💼 경력

<details open>
<summary><b>BIND</b> &nbsp;<code>2026.01 ~ 재직 중</code> &nbsp;·&nbsp; Python · Django · Celery · Redis · AWS</summary>

<br/>

- **인스타그램 게시물 자동 수집 파이프라인** — Redis 분산락으로 중복 수집 차단, 미디어를 8MB 청크로 S3 스트리밍 업로드. 어드민 수동 등록 `0건` 전환, 노출 지연 `1~2일 → 24시간 이내`
- **HLS 영상 변환 파이프라인** — AWS MediaConvert를 검토 후 폐기, ffmpeg + Celery로 직접 구축. 100MB 원본을 2MB 미만 6초 segment로 분할해 모바일 점진 재생
- **전화번호 인증 백엔드 이관** — 검증을 프론트에서 서버로 이관, Redis 레이트리밋(시간당 10회)으로 SMS 비용·우회 차단. 테스트 `213개` 작성

</details>

<details>
<summary><b>위밋모빌리티</b> &nbsp;<code>2024.10 ~ 2026.01</code> &nbsp;·&nbsp; Kotlin · Spring Boot · JPA · Querydsl · Kubernetes · K6</summary>

<br/>

- **대용량 주문 처리 재설계** `60초 → 3~5초` — SQS 비동기를 API 직접 처리로 전환, 임시테이블 제거. 단일 순회 추출 + HashMap 조회 + BatchInsert로 재구성
- **주기적 서버 다운 진단** `1,200ms → 55ms` — Grafana·CloudWatch로 다운 패턴 분석, Slow Query 진단 후 풀스캔성 쿼리 분할·페이지네이션 적용
- **CI 테스트 속도 개선** `3분 20초 → 21초` — 700개 넘는 테스트를 병렬 실행으로 전환, MockK 중복 주입을 BaseUnitTest로 통합
- **서버 스케일 조정** — K6로 Vuser 1,000까지 부하 측정, Pod당 리소스를 줄이고 12개로 분산해 피크 시간대 `timeout 0건`

</details>

<details>
<summary><b>라이너스</b> &nbsp;<code>2023.07 ~ 2024.09</code> &nbsp;·&nbsp; Kotlin · Spring · 코루틴 · 배치</summary>

<br/>

- **외부 API 호출 사전 적재 재설계** `42초 → 20ms` — 반복 호출 개선(42→10초) → 코루틴 병렬화(10→3초) → 30분 단위 배치 사전 적재(3초→20ms). 외부 서비스 의존을 구조적으로 제거
- **서버 분리로 webhook 유실 방지** `유실률 0%` — 줌·파놉토·과제 집계 서버를 분리해 webhook 수신 격리, 테스트 코드·PR 리뷰 규칙 도입

</details>

<details>
<summary><b>그 외</b> &nbsp;·&nbsp; 레인보우8 · 쿠돈 · 빅스텝에듀케이션</summary>

<br/>

- **레인보우8** `2021.12 ~ 2022.11` — PHP 홈페이지를 Java·Spring으로 마이그레이션, 러시아 IP 스팸메일(일 100여 건)을 reCAPTCHA로 차단, 배포 없는 공지 배너 API 운영
- **쿠돈** `2021.07 ~ 2021.10` — 쿠폰 1회 사용 보장 로직 구현, 매일 20:00 배송 확인 Job으로 구매 확정 알림톡 자동화
- **빅스텝에듀케이션** `2021.05 ~ 2021.06` — 인턴 팀으로 한 달간 멘토링 플랫폼 MVP 출시 (JWT · Django · S3)

</details>

<br/>

## 🛠️ 기술 스택

<table>
<tr>
<td><b>주력</b></td>
<td>
<img src="https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white" />
<img src="https://img.shields.io/badge/Java-0F172A?style=flat-square&logo=openjdk&logoColor=white" />
<img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white" />
<img src="https://img.shields.io/badge/JPA_·_Querydsl-59666C?style=flat-square&logo=hibernate&logoColor=white" />
</td>
</tr>
<tr>
<td><b>병행</b></td>
<td>
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white" />
<img src="https://img.shields.io/badge/Celery-37814A?style=flat-square&logo=celery&logoColor=white" />
<img src="https://img.shields.io/badge/Spring_Batch-6DB33F?style=flat-square&logo=spring&logoColor=white" />
</td>
</tr>
<tr>
<td><b>데이터</b></td>
<td>
<img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white" />
<img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" />
</td>
</tr>
<tr>
<td><b>인프라</b></td>
<td>
<img src="https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white" />
<img src="https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white" />
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
<img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" />
<img src="https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white" />
<img src="https://img.shields.io/badge/K6-7D64FF?style=flat-square&logo=k6&logoColor=white" />
</td>
</tr>
</table>

<br/>

<div align="center">
<sub>전남대학교 경제학과 학사 &nbsp;·&nbsp; 총 경력 5년 1개월 &nbsp;·&nbsp; 기술 선택 과정은 <a href="https://gyungjae-ham.github.io">블로그</a>에 기록합니다.</sub>
</div>
