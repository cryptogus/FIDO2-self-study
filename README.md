# FIDO

by chatGPT

"FIDO"는 "Fast IDentity Online"의 약자로, 온라인 인증 표준을 개발하는 FIDO Alliance라는 조직이 만든 용어. https://fidoalliance.org/?lang=ko

 FIDO 표준은 비밀번호 기반 인증의 단점을 극복하고자 만들어졌으며, 더 안전하고 사용하기 쉬운 인증 방법을 제공합니다. FIDO는 주로 생체 인식(지문, 얼굴 인식 등)이나 보안 키 같은 물리적 장치를 사용하여 인증을 수행합니다.

### 주요 특징:
1. **비밀번호 없는 인증:** FIDO는 비밀번호 대신 생체 인식 데이터나 보안 키를 사용합니다.
2. **강력한 보안:** 공용 키 암호화를 사용하여 사용자 데이터를 보호하며, 인증 과정에서 사용자 정보를 서버에 저장하지 않습니다.
3. **편리성:** 사용자는 복잡한 비밀번호를 기억할 필요 없이 손쉽게 인증할 수 있습니다.
4. **호환성:** 다양한 장치와 플랫폼에서 사용 가능합니다.

### FIDO의 구성 요소:
1. **FIDO UAF (Universal Authentication Framework):** 비밀번호 없이 생체 인식 데이터나 PIN을 사용하여 사용자 인증을 수행합니다.
2. **FIDO U2F (Universal 2nd Factor):** 비밀번호와 함께 사용하는 두 번째 인증 수단으로 보안 키를 사용합니다.
3. **FIDO2:** FIDO UAF와 U2F의 장점을 결합하여 비밀번호 없는 인증을 지원하는 최신 표준입니다. 웹 인증(WebAuthn)과 클라이언트-인증자(Client-to-Authenticator) 프로토콜(CTAP)을 포함합니다.

FIDO 표준을 채택하면 사용자 경험이 개선되고, 보안 위협에 대한 저항력이 높아져 많은 기업과 서비스에서 점점 더 많이 도입되고 있습니다.

FIDO(Fast IDentity Online) 인증 표준이 안전한 이유는 다음과 같은 주요 보안 특징들에 기반합니다:

### 1. 공개 키 암호화 사용
FIDO는 공개 키 암호화(Public Key Cryptography)를 사용합니다. 이 방식에서는 사용자 디바이스에서 생성된 개인 키(Private Key)와 공개 키(Public Key) 쌍을 사용하여 인증을 수행합니다.
- **개인 키**는 사용자 디바이스에 안전하게 저장되고 절대 디바이스 밖으로 노출되지 않습니다.
- **공개 키**는 서비스 제공자에게 전달되며, 이 키를 사용하여 사용자 인증 요청을 검증합니다.

### 2. 생체 인식 데이터의 안전한 처리
FIDO는 지문, 얼굴 인식 등 생체 인식 데이터를 사용하더라도, 이러한 민감한 데이터가 디바이스를 벗어나지 않도록 설계되어 있습니다.
- 생체 인식 데이터는 로컬 디바이스에서만 처리되고 저장됩니다.
- 인증 시 생체 인식 데이터는 개인 키를 활성화하는 데 사용되며, 생체 인식 데이터 자체가 서버로 전송되지 않습니다.

### 3. 피싱 공격 방지
FIDO는 사용자가 인증할 때마다 고유한 인증 정보를 생성합니다. 이는 피싱 공격을 방지하는 데 도움이 됩니다.
- 공격자가 피싱 웹사이트를 통해 인증 정보를 가로채려 해도, 해당 정보는 고유하고 일회성(One-Time Use)이기 때문에 유효하지 않습니다.

### 4. 중간자 공격 방지
FIDO의 인증 과정은 도중에 가로챌 수 없는 안전한 채널을 통해 이루어집니다. 사용자와 서비스 제공자 간의 통신이 암호화되어 중간자(Man-in-the-Middle) 공격에 대한 저항력이 높습니다.

### 5. 보안 장치 활용
FIDO 인증은 보안 장치(Security Key)를 사용할 수 있습니다. 이러한 장치는 하드웨어 기반의 보안 요소를 제공하여 높은 수준의 보안을 보장합니다.
- 보안 장치는 개인 키를 하드웨어 내에서 안전하게 저장하고, 물리적 접근 없이는 개인 키를 추출할 수 없습니다.
- 보안 장치는 사용자가 물리적으로 소유하고 있기 때문에, 원격으로 탈취가 어렵습니다.

### 6. 다중 요소 인증
FIDO는 다중 요소 인증(Multi-Factor Authentication, MFA)을 지원하여 보안을 한층 강화합니다.
- 사용자는 생체 인식과 함께 PIN이나 비밀번호 같은 추가 요소를 사용할 수 있습니다.
- 여러 가지 인증 요소를 결합하여 단일 요소에 비해 보안이 강화됩니다.

### 요약
FIDO는 공개 키 암호화, 생체 인식 데이터의 로컬 처리, 피싱 및 중간자 공격 방지, 보안 장치 사용, 다중 요소 인증 등을 통해 높은 수준의 보안을 제공합니다. 이러한 특징들은 사용자 데이터의 안전을 보장하고, 비밀번호 기반 인증의 취약점을 극복하는 데 기여합니다.
## FIDO Librarys

https://developers.yubico.com/Software_Projects/

https://github.com/solokeys/solo1\
https://github.com/solokeys/solo1-cli\
https://github.com/solokeys/solo2\
https://github.com/solokeys/solo2-cli