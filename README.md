# 정수리 독수리 연구소 — 공개 사이트 올리기

준비물: GitHub 계정, Google 계정 (Firebase 무료 요금제로 충분해요). 시간은 20분쯤 걸려요.

## 1. Firebase 프로젝트 만들기 (데이터·로그인 담당)
1. https://console.firebase.google.com → **프로젝트 추가** → 이름 `jeongsuri-lab` (애널리틱스는 꺼도 돼요)
2. 왼쪽 **빌드 > Authentication** → 시작하기 → 로그인 방법에서 **이메일/비밀번호** 사용 설정
3. **빌드 > Firestore Database** → 데이터베이스 만들기 → 위치 `europe-west1 (Belgium)` → **프로덕션 모드**
   - **규칙** 탭에 `firestore.rules` 내용을 통째로 붙여 넣고 **게시**
4. **빌드 > Realtime Database** → 데이터베이스 만들기 → 위치 `europe-west1` → **잠금 모드**
   - **규칙** 탭에 `database.rules.json` 내용을 붙여 넣고 **게시**
5. 프로젝트 개요 옆 톱니 → **프로젝트 설정** → 아래 **내 앱**에서 웹 아이콘 `</>` → 앱 등록
   - 나오는 `firebaseConfig` 값들을 `config.js`의 `firebase: { ... }` 안에 붙여 넣기
   - `databaseURL`이 안 보이면 Realtime Database 화면 위쪽 주소(https://…firebasedatabase.app)를 넣으세요

## 2. GitHub Pages에 올리기 (사이트 담당)
1. GitHub → **New repository** → 이름 예: `jeongsuri-lab` → **Public** → Create
2. **Add file > Upload files** → 이 폴더의 `index.html`, `config.js`, `fonts` 폴더를 끌어다 놓기 → Commit
3. 저장소 **Settings > Pages** → Source: **Deploy from a branch**, Branch: `main` / `(root)` → Save
4. 1~2분 뒤 주소가 나와요: `https://<깃허브아이디>.github.io/jeongsuri-lab/`
5. Firebase **Authentication > 설정 > 승인된 도메인**에 `<깃허브아이디>.github.io` 추가

## 3. 벨라에게 개발자 권한 주기
1. 사이트에 들어가서 **처음 왔어요 · 가입하기** → 별명 `벨라`, 비밀번호 4자리로 가입
2. **나의 연구 여정** 창 맨 아래 **내 계정 ID**를 복사
3. `config.js`의 `ownerUid: ""` 따옴표 안에 붙여 넣고 GitHub에 다시 업로드
4. Firebase Firestore **규칙**에서 `'OWNER_UID'`를 같은 ID로 바꾸고 **게시**
5. 새로고침하면 화이트보드 공지, 네온 문구, 피드백 확인 같은 개발자 기능이 열려요

## 알아 둘 것
- `config.js`의 Firebase 값은 공개돼도 괜찮아요. 누가 무엇을 쓸 수 있는지는 위 규칙이 지켜요.
- 비밀번호가 숫자 4자리라 강하지 않아요. Firebase가 반복 시도를 막고, 사이트도 5번 틀리면 30초 잠가요. 그래도 중요한 정보는 넣지 마세요.
- 온글잎 승훈체는 웹사이트에 올려 써도 되는지 라이선스를 한 번 확인해 주세요.
- 고칠 때는 `index.html`만 다시 올리면 돼요.
