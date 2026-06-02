# WebBlender - 웹 기반 3D 에디터

Blender 수준의 기능을 웹 브라우저에서 제공하는 3D 제작 프로그램입니다.  
설치 없이 GitHub Pages에서 바로 실행됩니다.

## 🚀 GitHub Pages 배포 방법

1. **이 저장소를 Fork** 또는 새 저장소 생성 후 `index.html` 업로드
2. **Settings → Pages → Branch: main / root** 선택 후 Save
3. `https://[username].github.io/[repo-name]/` 에서 실행

## ✅ 구현된 기능

### Viewport
- **Orbit**: Alt+드래그 (또는 중클릭+드래그)
- **Pan**: Shift+우클릭+드래그
- **Zoom**: 마우스 휠
- **Perspective / Orthographic** 전환
- **Grid & Gizmo** 오버레이
- **Wireframe / Solid / Material / Rendered** 뷰포트 모드

### 씬 계층 (Outliner)
- Object Tree / 가시성 토글 / 검색 / 선택

### 오브젝트 추가 (Shift+A)
- Cube, Sphere, Plane, Cylinder, Cone, Torus
- Point / Spot / Directional Light
- Camera

### 변환 (Transform)
- **G** - Move (이동)
- **R** - Rotate (회전)
- **S** - Scale (스케일)
- **X/Y/Z** - 축 고정 (변환 중)
- **Shift+D** - Duplicate
- **Delete/X** - 삭제

### Edit Mode
- **Tab** - Object/Edit Mode 전환
- Vertex / Edge / Face 선택 모드
- Extrude / Inset / Subdivide / Loop Cut

### 머티리얼 시스템
- Color / Roughness / Metallic / Emission / Opacity
- 실시간 미리보기

### 애니메이션
- Timeline / Keyframe / Auto Key
- Play / Pause / Loop / 재생 속도
- **Space** - 재생/정지

### 카메라 뷰
- **Numpad 1** - Front
- **Numpad 3** - Side
- **Numpad 7** - Top
- **Numpad 0** - Camera
- **Home** - Frame All

### 렌더링
- **F12** - Render Image
- PNG / JPEG 내보내기

### 프로젝트
- Ctrl+S - 저장 (브라우저 로컬스토리지)
- Ctrl+O - 불러오기
- OBJ / JSON 내보내기
- 5분마다 자동 저장

### 편집
- **Ctrl+Z** - Undo
- **Ctrl+Y** / Ctrl+Shift+Z - Redo

## 🛠 기술 스택

| 분야 | 기술 |
|------|------|
| 3D Engine | Three.js r128 (CDN) |
| Rendering | WebGL 2.0 |
| UI | Vanilla CSS (dark theme) |
| State | JavaScript (plain) |
| 배포 | GitHub Pages (정적) |

## 📦 단일 파일

`index.html` 하나로 모든 기능이 동작합니다.  
외부 의존성: Three.js CDN만 필요 (자동 로드).

## 🗺 로드맵 (향후 개발)

- [ ] React + TypeScript 마이그레이션
- [ ] Zustand 상태 관리
- [ ] GLTF/FBX 완전 임포트
- [ ] Node 기반 Material Editor
- [ ] WebGPU Path Tracing
- [ ] 협업 (WebSocket)
- [ ] 클라우드 렌더링
- [ ] Python-like 플러그인 API
- [ ] Asset Browser

## 📄 라이선스

MIT License
