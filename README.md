# Mini Project

## 1. 프로젝트 개요

### 프로젝트 이름  
**헬쓱해요(Healthcare)**

### 프로젝트 설명  
**프로젝트 선정 이유**  
- 수업 내용을 기반
- 정리된 카테고리 필요
- 필요하다고 느낀 서비스 

**프로젝트 의도 및 목표**  
- **의도**: 현재까지 배운 Java, DB, JDBC에 대한 복습과 숙달  
- **목표**: 현재까지 배운 코드들을 사용하여 최대한 완벽에 가깝게 프로그램을 구동하는 것 

**기대 효과 및 주제 선정 이유**  
- 프로그램을 사용하는 회원들이 꾸준히 목표를 세우고 본인이 세운 목표를 이루며 본인의 건강을 관리하게끔 함  
- 시간을 내서 운동할 여력이 없는 바쁜 현대인들에게 구체적이고 체계적인 데이터들을 제공하여 건강 관리에 소홀해지지 않게 만들어 주기 위함  

---

## 2. 팀원 및 팀 소개

| 이수연 | 서종범 | 이진혁 | 최은서 |
|:------:|:------:|:------:|:------:|
| <img src="https://i.pinimg.com/enabled_lo_mid/736x/5e/6c/ab/5e6cab0c7e22c88232977228c56301f8.jpg" alt="이수연" width="150" height="150"> | <img src="https://i.pinimg.com/736x/e3/1e/fc/e31efc742b7bb4876d5011459cf88c46.jpg" alt="서종범" width="150" height="150"> | <img src="https://i.pinimg.com/736x/16/9f/3e/169f3e68827b047efc27f048b2d44049.jpg" alt="이진혁" width="150" height="150"> | <img src="https://i.pinimg.com/736x/d9/4e/8c/d94e8c6d7149857e686a56847d6dc932.jpg" alt="최은서" width="150" height="150"> |
| BE | PL | BE | BE |
| [GitHub](https://github.com/javapyhtml) | [GitHub](https://github.com/) | [GitHub](https://github.com/) | [GitHub](https://github.com/) |

---

## 3. 주요 기능

**BMI 설정**,
**운동 목표 설정**,
**운동 기록 설정**,
**식단 관리**,
**내 프로필**

---

## 4. 작업 및 역할 분담

| 이름 | 역할 | 담당 작업 |
|-----------------|-----------------|-----------------|
| **이수연** | 백엔드 + 발표 | BMI 설정, 식단 관리, 발표자료 제작 및 발표 |
| **서종범** | 프로젝트 총괄 | 운동 기록 설정, 프로젝트 코드 총 정리 |
| **이진혁** | 백엔드 | 운동 목표 설정 및 회원가입 |
| **최은서** | 디자인 | 내 프로필 담당 및 로고 |

---

## 5. 기술 스택

### 5.1 Language  
- **Java**

### 5.2 Frontend  
- IntelliJ IDEA  

### 5.3 Backend  
- Java  
- Oracle Database  
 
---

## 6. 벤치마킹 사례

- **삼성 헬스**
- **NOOM**  
- **샤오미 MiBand**  
- **FatSecret**
- **아이폰 건강** 

---

## 7. 프로젝트 구조

```plaintext
# 6. Project Structure (프로젝트 구조)
project/
├── src/
│   ├── Util/         # 유틸 클래스
│   │   ├── ExUtil.java        // 프로젝트 연결 설정
│   │   ├── BmiUtil.java       // BMI 설정 유틸
│   │   ├── GoalsUtil.java     // 운동 목표 설정 유틸
│   │   ├── MemberUtil.java    // 회원 관리 설정 유틸
│   │   ├── MenuUtil.java      // 식단 관리 설정 유틸
│   │   ├── RecordUtil.java    // 운동 기록 설정 유틸
│   │   ├── GraphUtility.java  // 그래프 유틸
│   │   │   ├── GraphPanel.class         // 그래프 패널
│   │   │   ├── GraphUtility.java        // 그래프 설정 유틸리티
│   ├── ExDAO/                  # 데이터 접근 계층
│   │   │   │   │   ├── ExSQL.java       // 데이터베이스 sql 
│   │   │   │   │   ├── Calender.java    // 달력
│   │   │   │   │   ├── Color.java       // 색상
│   ├── ExDTO/                  # 데이터 전송 객체
│   │   │   │   │   ├── EMember.java            // 회원 관리 객체
│   │   │   │   │   ├── EBMI.java               // BMI 관련 객체
│   │   │   │   │   ├── E_Menu.java             // 식단 관리 음식 객체 1 
│   │   │   │   │   ├── EFood.java              // 식단 관리 음식 객체 2
│   │   │   │   │   ├── EGoals.java             // 운동 목표 설정 객체
│   │   │   │   │   ├── ERecords.java           // 운동 기록 설정 객체
│   │   │   │   │   ├── ExTypes.java            // 운동 종류 설정 객체
│   ├── ExMain/             # 메인
│   │   │   │   │   ├── Main.java               // 메인
├── .gitignore                   # Git 무시 파일 목록
├── README.md                    # 프로젝트 개요 및 사용법
