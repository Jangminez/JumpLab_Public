# Jump Lab

이 프로젝트는 여러 기능들을 만들어 본 간단한 실험실 같은 느낌의 프로젝트입니다.  
플레이어는 다양한 아이템을 획득하고, 장착하거나 소비하며 스탯을 강화할 수 있습니다.  
아이템 슬롯과 툴바 시스템을 통해 직관적인 아이템 관리가 가능합니다.

## 주요 기능

### 1. 아이템 및 툴바 시스템 (ToolBar.cs, GameManager.cs)

- **아이템 슬롯 관리:** 여러 개의 아이템 슬롯을 통해 아이템을 분배하고 선택할 수 있습니다.  
- **아이템 획득 및 드롭:** 새로운 아이템 획득 시 슬롯에 자동 추가, 슬롯이 꽉 찼으면 자동으로 드롭 처리  
- **아이템 사용:** 소모품 아이템은 효과 적용 후 일정 시간 동안 지속, 장착형 아이템은 장착/해제 가능  
- **아이템 UI 표시:** 선택한 아이템의 프리팹을 화면에 보여주고, 아이템 정보를 UI에 표시  
- **Input System 연동:** 숫자키로 슬롯 선택 가능

### 2. 플레이어
- **PlayerController**: PlayerInput을 통해 플레이어의 조작을 관리 (이동, 점프, 상호작용 등)
- **PlayerStats**: 플레이어의 스탯을 관리
- **PlayerInteractor**: RayCasting을 활용해 오브젝트와의 상호작용 관리
- **PlayerEventHandler**: 플레이어와 관련된 Event를 한 곳에 모아서 사용
- **Player**: 위 스크립트들을 관리
### 3. UI (UIManager.cs)

- **체력 및 스태미너 바:** 실시간으로 상태 변화 반영  
- **피격 시 시각적 피드백:** 화면 깜빡임 효과  
- **아이템 정보 UI:** 상호작용 중인 아이템의 이름과 설명을 표시

### 4. 플랫폼 (JumpingPlatform.cs, MovingPlatform.cs)

- **JumpingPlatform:** 충돌 시 위로 점프시키는 점프패드  
- **MovingPlatform:** 설정된 구간을 반복 이동하며, 플랫폼 위에 있는 Rigidbody 오브젝트를 함께 이동시킴

## 조작법
- **이동**: `W`, `A`, `S`, `D`
- **점프**: `Space Bar`
- **상호작용**: `E`
- **슬롯 선택**: `1` ~ `0`
- **아이템 사용**: `마우스 우클릭`
- **매달리기**: `G`

---



https://github.com/user-attachments/assets/1f879592-94f0-4180-91b1-f6dae2ff5305




https://github.com/user-attachments/assets/0cd488a3-3af8-45bb-80b9-42babb4bb96a



