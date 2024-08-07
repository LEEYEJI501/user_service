# user_service

## 주요 기능
### 사용자 등록
- **회원가입** 
  - RegisterUserRequest 요청을 처리하여 새로운 사용자 등록
  - 사용자명 중복 체크 / 프로필 이미지와 사용자 정보 저장

- **이미지 저장** : 사용자의 프로필 이미지 정보를 데이터베이스에 저장
- **프로필 저장**  : 사용자의 프로필 정보를 Profile 엔터티로 저장하여 사용자와 연결
### 비밀번호 관리
- **비밀번호 해시화** : 사용자 비밀번호를 해시화하여 데이터베이스에 저장
- **비밀번호 검증** : 입력된 비밀번호가 저장된 해시화된 비밀번호와 일치하는지 확인
- **비밀번호 변경** : 사용자는 현재 비밀번호 입력 후 새로운 비밀번호로 변경 가능
### 사용자 검색 및 인증
- **사용자 검색** : 사용자 ID로 사용자를 검색하여 반환
- **사용자명 체크** : 사용자명이 이미 존재하는지 확인
- **사용자 인증** : 사용자명과 비밀번호를 입력받아 인증 처리
### 프로필 업데이트
- **프로필 업데이트** : 사용자의 프로필 정보 업데이트 / 새로운 이미지 정보를 포함하여 갱신
