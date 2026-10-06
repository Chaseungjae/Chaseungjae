<h1 align="center">차승재 · Game Developer</h1>

<p align="center">
  Unity · Godot · GameMaker 로 <b>직접 만들고, 직접 고친</b> 게임들을 모았습니다.<br/>
  기능 구현뿐 아니라 <b>버그의 원인을 코드에서 찾아 수정한 과정</b>을 각 프로젝트에 정리했습니다.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Unity-000000?style=for-the-badge&logo=unity&logoColor=white" />
  <img src="https://img.shields.io/badge/C%23-512BD4?style=for-the-badge&logo=csharp&logoColor=white" />
  <img src="https://img.shields.io/badge/Godot-478CBF?style=for-the-badge&logo=godotengine&logoColor=white" />
  <img src="https://img.shields.io/badge/GameMaker-000000?style=for-the-badge&logo=gamemaker&logoColor=white" />
  <img src="https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=cplusplus&logoColor=white" />
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" />
</p>

<p align="center">
  📧 <a href="mailto:jea353011@gmail.com">jea353011@gmail.com</a>
</p>

---

## 🎮 Projects

| 프로젝트 | 장르 / 엔진 | 인원 | 내가 한 일 | 링크 |
|---|---|---|---|---|
| **AETHERIS** | 2D 액션 로그라이크 / Unity 6 | 3인 | 스킬 시스템(10여 종), 스킬 트리, 아이템·창고, 보스 패턴, 파칭코 미니게임, 던전 분위기 연출 | [Repo](https://github.com/ksw-0409/NEW_PROJECT) · [Video](https://youtu.be/38FY_WGQWFs) |
| **God Is Death 2** | 보스 러시 액션 / GameMaker (GML) | 3인 | 보스 패턴·스킬, 공격 예고(텔레그래프) 시스템, 블랙홀 중력장 | [Repo](https://github.com/retser0319/GayMakerStudio) · [Video](https://youtu.be/cPjAl8rbP_c) |
| **지하철 호러 게임** | 3D 이상현상 호러 / Unity | 4인 | 1인칭 이동·카메라, 몬스터 AI·점프스퀘어 연출, 조명 연출, 버그 수정 | [Repo](https://github.com/Chaseungjae/UnityProject) · [Video](https://youtu.be/jdeIvBlqOUw) |
| **2D 액션 플랫포머** | 홀드 점프 플랫포머 / Godot 4 | 1인 | 기획부터 전체 구현 (차지 점프, 벽 반사 물리, 위험 타일 넉백) | [Repo](https://github.com/Chaseungjae/2Dproject) · [Video](https://youtu.be/_SWh5Mbt__I) |

---

## 🛠 Bug-fix highlights

실제 커밋에서 원인을 찾아 고친 사례 일부입니다.

- **보스가 체력 0이 되어도 죽지 않던 문제** *(GameMaker)* — 처치 판정 코드 누락을 찾아 `instance_destroy` 처리 + 보상 룸 전환 추가
- **보스 페이즈 2에서도 공격 속도가 그대로였던 문제** *(GameMaker)* — 쿨다운 하드코딩을 페이즈별 변수로 분리
- **적이 없어도 공격 스킬이 허공에 발동되던 문제** *(Unity)* — `SkillBase`에 가상 메서드(`RequiresEnemiesToCast`)를 추가해 방어 스킬만 예외 처리
- **보스 레이저가 기둥과 플레이어를 동시에 관통하면 무피해 처리되던 판정 버그** *(Unity)* — 빔 유지 시간 동안 프레임마다 충돌 재검사
- **대각선 이동 시 속도가 √2배 빨라지던 문제** *(Unity)* — 방향 벡터 합성 후 정규화
- **공격 애니메이션 중 몬스터가 미끄러지던 문제** *(Unity)* — 공격 시작 위치를 저장해 공격 중 고정

---

## 🧰 Skills

- **Unity / C#** — NavMesh AI, Cinemachine, URP 포스트프로세싱, 코루틴 기반 연출, 스킬·아이템 시스템 설계
- **Godot / GDScript** — 물리 기반 캐릭터 컨트롤러, 셰이더 배경
- **GameMaker / GML** — 알람 이벤트 기반 보스 패턴, 오브젝트 간 통신
- **C++** — 컴퓨터그래픽스 실습 ([lap](https://github.com/Chaseungjae/lap))
- **협업** — Git 브랜치/머지 기반 3~4인 팀 개발 경험
