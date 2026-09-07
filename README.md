<div align="center">

# DAVE THE DIVER Clone

<img src="docs/media/dave-the-diver-key-art.webp" width="620" alt="DAVE THE DIVER key art">

### C++17 · DirectX 9 Custom Engine · 4인 팀 프로젝트

**자체 제작 엔진으로 구현한 2D 해양 어드벤처·경영 게임 《데이브 더 다이버》 모작**

</div>

## 프로젝트 정보

| 항목 | 내용 |
| --- | --- |
| 장르 | 2D 횡스크롤 해양 어드벤처 · 경영 |
| 개발 기간 | 2026.01.31 ~ 2026.03.08 |
| 개발 인원 | 4명 |
| 플랫폼 | Windows x64 |
| 개발 환경 | Visual Studio · Windows SDK 10.0 |
| 제작 범위 | Engine · SRClient · Map/Debug Tools |
| 기술 스택 | • C++17<br>• DirectX 9 · DirectInput 8<br>• FMOD · Assimp 6.0.4 · Spine C++ 4.0<br>• Dear ImGui 1.83 · ImGuizmo<br>• nlohmann/json · Tweeny |

## 시연영상

[시연영상 보기](https://youtu.be/my8iDHUOXAk)

## 주요 콘텐츠

- 선박 준비 → 수중 탐험·어획 → 귀환·정산 → 초밥집 운영으로 이어지는 플레이 루프
- 작살 QTE와 근접 무기·총기를 활용한 물고기 포획 및 수중 전투
- 산소·수심·적재 중량 관리와 물고기·재료·장비 수집
- 돌진·사격·유도탄·폭발 패턴으로 구성된 2페이즈 보스전
- 인벤토리와 산소통·잠수복·화물함·작살 및 무기 업그레이드
- 메뉴 구성·요리 강화·와사비 준비·초밥과 차 서빙으로 진행되는 초밥집 경영

## 담당 파트

<table>
  <thead>
    <tr>
      <th>팀원</th>
      <th>담당 파트</th>
      <th>구현 내용</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <a href="https://github.com/ForestMS1"><strong>ForestMS1</strong></a>
      </td>
      <td>Player · Combat/Boss</td>
      <td>
        <strong>핵심 시스템</strong><br>
        • 플레이어 FSM·8방향 이동·카메라<br>
        • 작살·총기·근접 공격·Projectile·Fight QTE<br>
        <br>
        <strong>콘텐츠 구현</strong><br>
        • 산소·피격·사망·잠수함·무기 전환<br>
        • John → John2 2페이즈 보스와 전투 패턴
      </td>
    </tr>
    <tr>
      <td>
        <a href="https://github.com/gnffk"><strong>gnffk</strong></a>
      </td>
      <td>Map · Rendering/VFX</td>
      <td>
        <strong>핵심 시스템</strong><br>
        • MapMgr·JSON Save/Load·Terrain·Map Collision<br>
        • Frustum Culling·GLB Rendering·Light·Fog<br>
        <br>
        <strong>콘텐츠 구현</strong><br>
        • 수중 맵·산호·아이템·물고기 배치와 Map Editor<br>
        • 수심 기반 색감·조명·심해 및 수중 환경 파티클
      </td>
    </tr>
    <tr>
      <td>
        <a href="https://github.com/limits1214"><strong>limits1214</strong></a> · 임성윤
      </td>
      <td>Framework · Fish · UI</td>
      <td>
        <strong>핵심 시스템</strong><br>
        • GameObject·Layer·Scene·Component 생명주기<br>
        • AssetMgr·CollisionMgr·FMOD·UI 구성 및 Scene Transition<br>
        <br>
        <strong>콘텐츠 구현</strong><br>
        • 물고기 계층·어종·Spine 애니메이션·피격·충돌·QTE 포획<br>
        • 선박·iDiver·인벤토리·HUD·대화 및 게임 흐름 UI
      </td>
    </tr>
    <tr>
      <td>
        <a href="https://github.com/sungmin2ee"><strong>sungmin2ee</strong></a>
      </td>
      <td>Sushi · Particle</td>
      <td>
        <strong>핵심 시스템</strong><br>
        • ParticleMgr·PSystem·날씨·폭죽 VFX<br>
        • 손님·레시피·서빙·요리 강화·매장 운영 흐름<br>
        <br>
        <strong>콘텐츠 구현</strong><br>
        • 초밥집·메뉴 구성·와사비 준비·차 및 초밥 서빙<br>
        • 날씨·폭죽·엔딩·장면 전환 파티클 및 이펙트
      </td>
    </tr>
  </tbody>
</table>
