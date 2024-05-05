### 1. Broken Access Control

취약한 접근 제어 <br>
공격자가 사용자 또는 관리자 계정에 대한 액세스 권한을 사용하여 무단으로 데이터를 사용 -> 사용자가 권한을 벗어나 행동할 수 없도록 정책 지정

### 2. Cryptographic Failures

암호화 실패 <br>
평문으로 전송, 안전하지 않은 암호화 알고리즘 선택, 키 관리의 미흡 등으로 인해 발생 -> 최신 버전의 안전한 알고리즘 사용

### 3. Injection

XSS 포함. 사용자가 전달하는 데이터를 조작해서 서버 측에서 명령어나 쿼리의 일부로 인식해 발생 -> 유효성 검사 등

### 4. Insecure Design

불안전한 설계 <br>
설계 단계에서 보안을 고려하지 않고 개발해 발생 -> 안전한 설계 패턴 및 아키텍처 중요

### 5. Security Misconfiguration

보안 구성 오류 <br>
보안을 고려하지 않은 설정으로 인해 발생

### 6. Vulnerable and Outdated Components

취약하고 구식의 구성 요소 <br>
취약한 버전 또는 지원이 종료된 버전 사용할 때 발생. 알려진 보안 결함에 노출되어 공격 위험 증가.

### 7. Identification and Authentication Failures

식별 및 인증 오류 <br>
인증 및 세션 관리의 미흡 등 -> 다중 인증 구현 등

### 8. Software and Data Integrity Failures

소프트웨어 및 데이터 무결성 오류 <br>
무결성 체크

### 9. Security Logging and Monitoring Failures

보안 로깅 및 모니터링 실패 <br>
공격 감지 및 대응을 위해서는 로깅 및 모니터링이 필요

### 10. Server - Side Request Forgery(SSRF)

서버 측 요청 변조 <br>
서버가 위조된 요청을 보내도록 하는 취약점(CSRF는 client) <br>
