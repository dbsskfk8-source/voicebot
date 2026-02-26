🎙️ Python Voice Chatbot
OpenAI와 음성 인식 기술을 결합하여 대화가 가능한 지능형 보이스봇입니다.

🏗️ 시스템 아키텍처

graph TD
    Mic[마이크 소리] --> STT[음성 인식]
    STT -->|텍스트 변환| Logic[@ch03_voicebot.py]
    Logic -->|GPT 응답| TTS[음성 합성]
    TTS --> Speaker[스피커 출력]
📂 핵심 코드 가이드

통합 로직: @ch03_voicebot.py 파일 하나에서 음성 입력, GPT 처리, 음성 출력을 모두 제어합니다.

의존성: @requirements.txt와 @packages.txt를 통해 필요한 라이브러리 환경을 구축합니다.
