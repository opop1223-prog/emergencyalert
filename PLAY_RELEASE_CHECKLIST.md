# 어디야 Google Play 배포 체크리스트

## 앱 정보
- 앱 이름: 어디야
- 패키지 이름: com.example.emergencyalert
- 버전: 1.0 (versionCode 1)
- 개인정보 처리방침: https://emergency-a2fb7.web.app/privacy.html

## 업로드 파일
- 서명된 AAB 경로: app/build/outputs/bundle/release/app-release.aab
- 업로드 키스토어: release-keystore.jks
- 키스토어 비밀번호 파일: keystore.properties
- `release-keystore.jks`와 `keystore.properties`는 반드시 따로 백업해야 합니다. 잃어버리면 같은 앱 업데이트가 어려워질 수 있습니다.

## Play Console에서 확인할 항목
- 개인정보 처리방침 URL 등록
- 데이터 보안 섹션 작성
- 위치 권한 사용 사유 작성
- SMS 권한 사용 사유 작성
- 앱 콘텐츠 등급 설문 작성
- 테스트 트랙 또는 프로덕션 트랙에 AAB 업로드
- 실제 기기에서 위치/SMS/Firebase 기록 테스트

## 권한 설명 메모
- 위치 권한: SOS 전송 시 현재 위치 확인
- SMS 권한: 보호자에게 긴급 문자 전송
- 네트워크 권한: Firebase 연결 상태 확인 및 긴급 기록 저장
