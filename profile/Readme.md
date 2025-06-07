# 🏢 Pangyo Coffee Legends - 스마트 오피스 AIoT 시스템

> **"1년 뒤 판교 스타벅스에서 모이자!"**  
> AI + IoT 기반의 스마트 오피스 시스템 구축 프로젝트

---

## 🧠 프로젝트 개요

AI 및 IoT 기술을 융합하여 **쾌적한 업무 환경**과 **효율적인 오피스 운영**을 구현하는 통합 솔루션입니다.  
실시간 센서 데이터, AI 분석, 자동화 제어, 대시보드 시각화를 통해 스마트 오피스를 실현합니다.

### 🎯 주요 기능

| 기능             | 설명                                                   |
| -------------- | ---------------------------------------------------- |
| 🌡️ 환경 센싱 및 저장 | 센서 데이터를 MQTT/Modbus로 수집하고 InfluxDB에 저장               |
| 🤖 AI 쾌적도 분석   | 온습도/CO₂ 기반 쾌적도 예측 모델                                 |
| 🌍 환경 모니터링     | 기기 관리, 룰 관리, 장소 관리 기능 제공                             |
| 🔐 출입 통제/근태 분석 | 출입 로그 기반 근무 시간 계산 및 이상 감지                            |
| 📊 ELK 로그 모니터링 | Filebeat → Logstash → Elasticsearch → Kibana 대시보드 구성 |
| 🗓️ 회의실 예약 시스템 | 예약, 입장, 노쇼, 연장 등 기능 통합                               |
| 💬 실시간 채팅/알림   | Stomp 기반 실시간 채팅 / 알림 팝업 구현                            |


---

## 🏗️ 시스템 아키텍처

![image](https://github.com/user-attachments/assets/35b29f09-cae4-4515-af45-f5da3282e229)

## ⚙️ 기술 스택

| 분류         | 사용 기술 |
|--------------|-----------|
| 📌 백엔드     | Spring Boot, Spring Security, Spring Cloud Config, JPA |
| 🎨 프론트엔드 | HTML, CSS, JavaScript (Vanilla), Bootstrap |
| 🛠️ 인프라     | Docker, Nginx, GitHub Actions |
| 💾 DB/저장소  | InfluxDB, MySQL, Elasticsearch, H2, Redis |
| 🧠 AI/분석     | Python, XGBoost, Pandas, FastAPI |
| 📡 실시간     | Stomp, MQTT, Rule Engine, RabbitMQ |
| 📊 로그 시스템| Filebeat, Logstash, Kibana (ELK) |

---

## 👥 팀원 소개

| 프로필 | 이름 | 담당 역할 | GitHub |
|--------|------|-----------|--------|
| <img src="https://github.com/dusen0528.png" width="50"/> | 최인호 | 쾌적도 AI · ELK 로그 · CI/CD · 통합 인프라 | [@dusen0528](https://github.com/dusen0528) |
| <img src="https://github.com/HyunSubb.png" width="50"/> | 신현섭 | 채팅 시스템 · 실시간 알림 | [@HyunSubb](https://github.com/HyunSubb) |
| <img src="https://github.com/rudduddl.png" width="50"/> | 김경영 | 출입 통제 · 근태 분석 | [@rudduddl](https://github.com/rudduddl) |
| <img src="https://github.com/Migong0311.png" width="50"/> | 김미성 | 근태 분석 · 리포트 · Gemini 기반 분석 | [@Migong0311](https://github.com/Migong0311) |
| <img src="https://github.com/oculusK.png" width="50"/> | 강승우 | 환경 모니터링 · 이상 탐지 · Rule Engine | [@oculusK](https://github.com/oculusK) |
| <img src="https://github.com/phh624.png" width="50"/> | 박형호 | 환경 모니터링 · IoT 서비스 · JS 연동 | [@phh624](https://github.com/phh624) |
| <img src="https://github.com/Jyurim.png" width="50"/> | 전유림 | 회의실 예약 · 알림 · 대시보드 | [@Jyurim](https://github.com/Jyurim) |
| <img src="https://github.com/LEMON4DE.png" width="50"/> | 김지윤 | 회의실 CRUD · 회의실 예약 건 입실 통합관리 · 통계 | [@LEMON4DE](https://github.com/LEMON4DE) |

---


