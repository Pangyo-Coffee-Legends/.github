# 🏢 Pangyo Coffee Legends - 스마트 오피스 AIoT 시스템

> **"1년 뒤 판교 스타벅스에서 모이자!"**  
> AI + IoT 기반의 스마트 오피스 시스템 구축 프로젝트

---

## 🧠 프로젝트 개요

AI 및 IoT 기술을 융합하여 **쾌적한 업무 환경**과 **효율적인 오피스 운영**을 구현하는 통합 솔루션입니다.  
실시간 센서 데이터, AI 분석, 자동화 제어, 대시보드 시각화를 통해 스마트 오피스를 실현합니다.

### 🎯 주요 기능

| 기능 | 설명 |
|------|------|
| 🌡️ 환경 센싱 및 저장 | 센서 데이터를 MQTT/Modbus로 수집하고 InfluxDB에 저장 |
| 🤖 AI 쾌적도 분석 | 온습도/CO₂ 기반 쾌적도 예측 모델 |
| 🔐 출입 통제/근태 분석 | 출입 로그 기반 근무 시간 계산 및 이상 감지 |
| 📊 ELK 로그 모니터링 | Filebeat → Logstash → Elasticsearch → Kibana 대시보드 구성 |
| 🗓️ 회의실 예약 시스템 | 예약, 입장, 노쇼, 연장 등 기능 통합 |
| 💬 실시간 채팅/알림 | WebSocket 기반 채팅, 알림 팝업 구현 |

---

## 👨‍👩‍👧‍👦 팀원 소개

| 이름 | 담당 역할 | GitHub |
|------|-----------|--------|
| **최인호** | 쾌적도 AI · ELK 로그 · CI/CD · 통합 인프라 | [@dusen0528](https://github.com/dusen0528) |
| **신현섭** | 채팅 시스템 · 실시간 알림 | [@HyunSubb](https://github.com/HyunSubb) |
| **김경영** | 출입 통제 · 근태 분석 | [@rudduddl](https://github.com/rudduddl) |
| **김미성** | 근태 분석 · 리포트 · Gemini 기반 분석 | [@Migong0311](https://github.com/Migong0311) |
| **강승우** | 환경 모니터링 · 이상 탐지 · Rule Engine | [@oculusK](https://github.com/oculusK) |
| **박형호** | 환경 모니터링 · IoT 서비스 · JS 연동 | [@phh624](https://github.com/phh624) |
| **전유림** | 회의실 예약 · 알림 · 대시보드 | [@Jyurim](https://github.com/Jyurim) |
| **김지윤** | 예약 예외처리 · 입실 코드 · 통계 | [@LEMON4DE](https://github.com/LEMON4DE) |

---

## 🏗️ 시스템 아키텍처

```plaintext
[센서/사용자] 
   ↓ MQTT/Modbus
[IoT 서버] → [InfluxDB] → [AI 모델 서버] → [대시보드/알림]
   ↘ 로그 → Filebeat → Logstash → Elasticsearch → Kibana
   ↘ 예약/출입 관리 → Spring Gateway → REST API
```

## ⚙️ 기술 스택

| 분류         | 사용 기술 |
|--------------|-----------|
| 📌 백엔드     | Spring Boot, Spring Security, Spring Cloud Config, JPA |
| 🎨 프론트엔드 | HTML, CSS, JavaScript (Vanilla), Bootstrap |
| 🛠️ 인프라     | Docker, Nginx, GitHub Actions, AWS EC2 |
| 💾 DB/저장소  | InfluxDB, MySQL, Elasticsearch |
| 🧠 AI/분석     | Python, XGBoost, Pandas, FastAPI |
| 📡 실시간     | WebSocket, MQTT, Rule Engine |
| 📊 로그 시스템| Filebeat, Logstash, Kibana (ELK) |

