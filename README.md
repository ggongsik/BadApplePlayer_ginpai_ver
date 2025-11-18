# BadApplePlayer_ginpai_ver
# 🚀 핵심 기능 (Key Features)
WebManipulator는 F2 키(또는 더블클릭)로 활성화되는 강력한 패널을 통해 웹페이지의 모든 요소를 실시간으로 제어합니다.

# 1. 🎨 실시간 비디오 렌더링 엔진
로컬 비디오 파일 하나로 웹페이지 전체를 미디어 아트로 변화시킵니다.

Video-to-ASCII (Bad Apple Player): 선택된 DOM 요소를 실시간 비디오-투-ASCII 아트로 변환합니다. (폰트 크기, 줄 간격, 자간 조절 가능)

Video-to-SVG (Graph): (가장 인상적인 기능) 페이지 내 SVG를 선택하면, 비디오 프레임의 **윤곽선(Contour)**을 실시간으로 추출하여 SVG의 path 데이터를 덮어씁니다.

Video Wall: 페이지의 모든 <img> 태그를 찾아 canvas로 교체한 뒤, 하나의 거대한 비디오를 분할 재생하여 '비디오 월'을 구현합니다.

Animated Favicon: 브라우저 탭의 파비콘을 선택한 비디오로 실시간 애니메이션화합니다.

Background Mode: 웹페이지 전체 배경을 재생 중인 비디오로 대체합니다.

Media Session API: OS 미디어 컨트롤러(잠금 화면, 알림 창)에 현재 재생 중인 비디오 프레임을 썸네일로 실시간 전송합니다.

# 2. 🌊 미디어 및 DOM 하이재킹
웹페이지의 기존 콘텐츠를 사용자가 원하는 미디어로 강제 교체합니다.

Replace All Videos: 페이지의 모든 <video>, <iframe>, <embed> 태그를 찾아 선택한 로컬 비디오로 일괄 교체합니다.

Replace All Images: 모든 <img> 태그를 선택한 비디오(재생) 또는 이미지로 교체합니다.

Div Mode: 특정 div를 선택하면, 비디오 프레임의 밝기 값에 따라 해당 div를 복제하여 픽셀 아트를 생성합니다.

# 3. 🛠️ 웹사이트 조작 및 디버깅
웹 개발 및 분석을 위한 강력한 유틸리티를 제공합니다.

Inspect Element (Overlay): 마우스를 올린 요소의 XPath, Tag, ID, Class, Shadow DOM 상태를 실시간으로 보여주는 미니 개발자 도구입니다.

Text Edit Mode: contentEditable 속성을 활성화하여 웹페이지의 모든 텍스트를 즉시 수정할 수 있습니다.

CSP Override: 페이지의 Content-Security-Policy를 제거하고 unsafe-inline을 허용하는 정책으로 덮어씁니다. (스크립트 작동을 위한 선행 조치)

RGB Mode: 선택한 텍스트 요소의 색상을 무지개색으로 실시간 애니메이션화합니다.

Kill Website: document.body.innerHTML을 비워 페이지의 모든 요소를 즉시 삭제합니다.

# 🛠️ 주요 기술 스택 (Technical Showcase)
이 프로젝트는 다음과 같은 브라우저 핵심 기술에 대한 숙련도를 올리기 위해 진행하였습니다..

Canvas 2D API: getImageData(), drawImage()를 활용한 실시간 프레임 분석, 픽셀 데이터(밝기, 엣지) 추출.

Web Media APIs: URL.createObjectURL()을 통한 로컬 파일 처리, <video> 요소 제어, navigator.mediaSession 연동.

Advanced DOM Manipulation: requestAnimationFrame 기반의 고성능 렌더링 루프, Shadow DOM 재귀 탐색, contentEditable 동적 활성화.

Web Security (Understanding): Content-Security-Policy 메타 태그의 동적 주입 및 제거 로직.

Performance: 다수의 실시간 렌더링 루프가 동시에 작동함에도 불구하고 requestAnimationFrame을 통해 브라우저 렌더링에 최적화.

# 💡 사용 방법 (How to Use)
Tampermonkey 또는 Greasemonkey와 같은 유저 스크립트 매니저를 설치합니다.

본 WebManipulator.user.js 스크립트를 설치합니다.

조작하고 싶은 웹페이지에 접속합니다.

F2 키 또는 마우스 더블클릭으로 제어 패널을 엽니다. (F3로 숨김)

기능을 적용할 대상(텍스트, 이미지, SVG 등)을 마우스 우클릭하여 선택합니다.

🗳 File 버튼으로 로컬 비디오(MP4) 파일을 불러옵니다.

원하는 기능의 버튼(예: ASCII Mode, Graph, Video Wall)을 클릭하여 실행합니다.
