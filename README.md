라사 카레하우스 매장 관리 시스템

카레 전문점을 위한 통합 매장 관리 시스템
재고 관리, 판매 등록, 생산 계획 관리

## 📋 프로젝트 소개

라사 카레하우스 매장 관리 시스템은 카레 전문점의 일상 업무를 효율적으로 관리할 수 있는 모바일 애플리케이션입니다. 판매 등록부터 재고 관리, 생산 계획까지 통합적으로 관리할 수 있는 솔루션을 제공합니다.

이 애플리케이션은 React Native로 개발되어 Android 플랫폼에서 사용할 수 있으며, 오프라인 환경에서도 원활하게 작동합니다.

## ✨ 주요 기능

- **인증 시스템**: 안전한 로그인 및 사용자 관리 ( 요번 프로젝트에서는 관리자 계정으로 진행 )
- **대시보드**: 매출, 재고, 생산 현황을 한눈에 파악
- **판매 관리**: 간편한 메뉴 선택 및 판매 등록, 커스텀 메뉴 추가 기능
- **재고 관리**: 카레, 음료 등 재고 실시간 확인 및 관리
- **생산 계획**: 재고 부족 시 자동 생산 계획 생성 및 진행 관리
- **다크/라이트 모드**: 사용 환경에 맞는 테마 설정

## 🛠️ 기술 스택

- **프론트엔드**: React Native, TypeScript
- **상태 관리**: Redux, Redux Toolkit
- **스타일링**: React Native StyleSheet
- **로컬 저장소**: AsyncStorage
- **API 통신**: Axios (목업 API 사용)

## 📁 프로젝트 구조

```
/src
  /components        # 재사용 가능한 UI 컴포넌트
    /common          # 공통 컴포넌트 (모달, 메뉴 등)
  /screens           # 주요 화면 컴포넌트
    /auth            # 인증 관련 화면
  /store             # Redux 상태 관리
    /slices          # Redux 슬라이스
  /services          # API 및 로컬 데이터 관리
  /utils             # 유틸리티 함수
  /types             # TypeScript 타입 정의
  /navigation        # 네비게이션 구성
```

## 🚀 주요 개선 사항

### 1. 대시보드 화면 개선
- 실제 판매/재고 데이터 반영 통계 구현
- 소수점 표시 최적화 (소수점 첫째 자리까지만 표시)
- 데이터 시각화 개선

### 2. 판매 등록 화면 개선
- 직관적인 제품 선택 UI 
- 카테고리별 필터링 및 검색 기능
- 새 메뉴 추가 기능 (현장에서 즉시 추가 가능)
- 수량 조절 UI 개선 (버튼 및 입력 필드 크기 최적화)
- 쇼핑카트 형태의 선택 제품 목록 인터페이스

### 3. 데이터 포맷 최적화
- 소수점 처리 유틸리티 함수 구현
- 화폐 및 수량 표시 일관성 유지
- 정수는 소수점 없이, 소수는 첫째 자리까지만 표시

### 4. 재고 관리 시스템 강화
- 제품 유형별 재고 차감 로직 개선 (커리, 음료, 콤보)
- 임시 추가 메뉴에 대한 재고 처리 방식 추가
- 재고 부족 시 자동 생산 계획 생성

## 📥 설치 및 실행 방법

### 요구 사항
- Node.js (14.x 이상)
- npm 또는 yarn
- React Native CLI
- iOS 개발: Xcode (Mac 필요)
- Android 개발: Android Studio

## 🖼️ 주요 화면

- **로그인 화면**
- **홈 화면**: 실시간 현황 및 주요 메뉴 접근

![수정](https://github.com/user-attachments/assets/b81e3431-d056-4104-90ba-c47b790d0ca8) ![홈화면 3](https://github.com/user-attachments/assets/1ecfc958-b044-474d-b9c1-133dff103aa8)

- **대시보드**: 매출 통계 및 차트

![대시보드_1](https://github.com/user-attachments/assets/c35ab8ca-44fd-4473-86d1-ee4babebda2c) ![대시보드_2](https://github.com/user-attachments/assets/2ee8452b-ac2c-4906-aa85-e75d3c4b9669) ![대시보드_3](https://github.com/user-attachments/assets/44d6a108-e6bd-42aa-8e75-7310d88a6565)

- **판매 등록**: 메뉴 선택 및 주문 생성

![판매등록1](https://github.com/user-attachments/assets/7802e5e5-8b9a-4868-9bac-cc1743618fb3) ![판매등록2](https://github.com/user-attachments/assets/ddca1c92-2009-4b3e-8112-53c371a199f6) ![판매등록3](https://github.com/user-attachments/assets/229985aa-4b6a-43d7-9f1d-3539500dccf8)

- **재고 관리**: 제품별 재고 확인 및 관리

![재고관리1](https://github.com/user-attachments/assets/11bf2ee3-cc32-4215-8b7d-a38db335ed41) ![재고](https://github.com/user-attachments/assets/396c3eaa-f570-4f29-a520-40efe5375a4e)

- **생산 계획**: 생산 일정 및 진행 상황 관리

![생산 관리 1](https://github.com/user-attachments/assets/59f631dc-5e05-4766-a275-6ae4c1176d4d) ![생산 관리 2](https://github.com/user-attachments/assets/3c57eefb-8de5-402d-ba96-ca0728d04c88)

## 🔒 인증 정보 (개발용)

개발 및 테스트 목적으로 다음 계정을 사용할 수 있습니다:
- 아이디: admin
- 비밀번호: password


