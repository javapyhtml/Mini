# Semi Project

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
| FE | PL | FE | FE |
| [GitHub](https://github.com/javapyhtml) | [GitHub](https://github.com/) | [GitHub](https://github.com/) | [GitHub](https://github.com/) |

---

## 3. 주요 기능

**BMI 설정**
**운동 목표 설정**
**운동 기록 설정**
**식단 관리**
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
│   ├── main/
│   │   ├── java/
│   │   │   ├── com.example.project/    # 패키지 디렉토리
│   │   │   │   ├── controllers/         # 컨트롤러 클래스
│   │   │   │   │   ├── BasicController.java       // 기본 기능 컨트롤러
│   │   │   │   │   ├── BoardController.java       // 게시판 관련 컨트롤러
│   │   │   │   │   ├── CommentController.java     // 댓글 관리 컨트롤러
│   │   │   │   │   ├── PageMoveController.java    // 페이지 이동 처리
│   │   │   │   │   ├── PlaylistController.java    // 재생목록 관리 컨트롤러
│   │   │   │   │   ├── RestfulController.java     // RESTful API 처리
│   │   │   │   │   ├── SearchController.java      // 검색 요청 처리
│   │   │   │   │   ├── UrlRedirectController.java // URL 리다이렉션 처리
│   │   │   │   │   ├── UserController.java        // 사용자 관리 컨트롤러
│   │   │   │   ├── dao/                  # 데이터 접근 계층
│   │   │   │   │   ├── ArtistDetailDAO.java       // 아티스트 데이터 접근 클래스
│   │   │   │   │   ├── BoardRepository.java       // 게시판 데이터 저장소
│   │   │   │   │   ├── CommentRepository.java     // 댓글 데이터 저장소
│   │   │   │   │   ├── MusicDetailDAO.java        // 음악 세부정보 접근 클래스
│   │   │   │   │   ├── PlaylistDAO.java           // 재생목록 데이터 접근 클래스
│   │   │   │   │   ├── PlaylistInfoDAO.java       // 재생목록 정보 데이터 접근
│   │   │   │   │   ├── UserDAO.java               // 사용자 데이터 접근 클래스
│   │   │   │   ├── dto/                  # 데이터 전송 객체 및 엔티티
│   │   │   │   │   ├── ArtistDetailDTO.java       // 아티스트 상세 데이터 전송 객체
│   │   │   │   │   ├── ArtistDetailEntity.java    // 아티스트 상세 데이터 엔티티
│   │   │   │   │   ├── BoardDTO.java              // 게시판 데이터 전송 객체
│   │   │   │   │   ├── BoardEntity.java           // 게시판 데이터 엔티티
│   │   │   │   │   ├── CommentDTO.java            // 댓글 데이터 전송 객체
│   │   │   │   │   ├── CommentEntity.java         // 댓글 데이터 엔티티
│   │   │   │   │   ├── MusicDetailDTO.java        // 음악 세부 데이터 전송 객체
│   │   │   │   │   ├── MusicDetailEntity.java     // 음악 세부 데이터 엔티티
│   │   │   │   │   ├── PlaylistDTO.java           // 재생목록 데이터 전송 객체
│   │   │   │   │   ├── PlaylistEntity.java        // 재생목록 데이터 엔티티
│   │   │   │   │   ├── PlaylistInfoDTO.java       // 재생목록 정보 데이터 전송 객체
│   │   │   │   │   ├── PlaylistInfoEntity.java    // 재생목록 정보 데이터 엔티티
│   │   │   │   │   ├── SearchDTO.java             // 검색 데이터 전송 객체
│   │   │   │   │   ├── UserDTO.java               // 사용자 데이터 전송 객체
│   │   │   │   │   ├── UserEntity.java            // 사용자 데이터 엔티티
│   │   │   │   ├── services/             # 서비스 계층
│   │   │   │   │   ├── ArtistService.java         // 아티스트 관련 서비스
│   │   │   │   │   ├── BoardService.java          // 게시판 관련 서비스
│   │   │   │   │   ├── CommentService.java        // 댓글 관리 서비스
│   │   │   │   │   ├── MusicService.java          // 음악 관리 서비스
│   │   │   │   │   ├── PlaylistService.java       // 재생목록 관리 서비스
│   │   │   │   │   ├── SearchService.java         // 검색 서비스
│   │   │   │   │   ├── UserService.java           // 사용자 관리 서비스
│   │   │   ├── resources/
│   │   │   │   ├── application.properties         // 환경 설정 파일
│   │   │   │   ├── static/                        # 정적 파일(css, js 등)
│   │   │   │   ├── templates/                     # HTML 템플릿 파일
│   │   │   │   │   ├── boardheader.html
│   │   │   │   │   ├── footer.html
│   │   │   │   │   ├── header.html
│   │   │   │   │   ├── index.html
│   │   │   │   │   ├── playlist.html
│   │   │   │   │   ├── test.html
│   │   │   │   │   ├── board/                     # 게시판 관련 템플릿
│   │   │   │   │   │   ├── list.html
│   │   │   │   │   │   ├── view.html
│   │   │   │   │   │   ├── write.html
│   │   │   │   │   ├── music/                     # 음악 관련 템플릿
│   │   │   │   │   │   ├── artistinfo.html
│   │   │   │   │   │   ├── playlistinfo.html
│   │   │   │   │   ├── top/                       # 장르별 TOP 50
│   │   │   │   │   │   ├── balledtop50.html
│   │   │   │   │   │   ├── bandtop50.html
│   │   │   │   │   │   ├── dancetop50.html
│   │   │   │   │   │   ├── hiphoptop50.html
│   │   │   │   │   │   ├── indietop50.html
│   │   │   │   │   │   ├── poptop50.html
│   │   │   │   │   │   ├── rbtop50.html
│   │   │   │   │   │   ├── trotop50.html
│   │   │   │   │   ├── user/                      # 사용자 관련 템플릿
│   │   │   │   │   │   ├── join.html
│   │   │   │   │   │   ├── login.html
│   │   │   │   │   │   ├── modlogin.html
│   │   │   │   │   │   ├── mypage.html
├── .gitignore                   # Git 무시 파일 목록
├── README.md                    # 프로젝트 개요 및 사용법
