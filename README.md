# T2_Korean_Patch-T2Fix_All-in-One-Pack
T2_Korean_Patch+T2Fix_All-in-One Pack NSIS 인스톨러 스크립트<br>
T2Fix 설치파일이 해당 파일들과 같은 디렉토리에 있어야하며, 한글패치는 최신본 압축해제한 상태로 같이 넣어서 패킹<br>

===========================
 Thief II : The Metal Age 한글 패치 v1.0
===========================

한글패치 제작 : 한국 씨프 카페
cafe.naver.com/thiefgame

한글화 총괄 : 제로방송 (coolgarlic@gmail.com)
번역 및 지원 : include, Sassy, Ospaggi


2026년 6월 26일 v1.0 : 한글패치 공개


===============
설치방법
===============
*올인원팩은 경로 설정만 해주면 아래 일체 과정을 알아서 진행합니다. 

1. 씨프2에 T2Fix 패치를 한다.(1.27 버전 이상 설치 권장)
- T2Fix 패치 주소 : https://cafe.naver.com/thiefgame/600
   * 씨프2 설치 경로
     ㆍ스팀판 : C:\Program Files (x86)\Steam\steamapps\common\thief_2
     ㆍGOG판 : C:\Program Files (x86)\GOG Galaxy\Games\Thief 2 - The Metal Age

   * T2Fix 설치 후 씨프2를 한번 실행했다가 종료하고,

2. 씨프2 한글패치 v1.0.zip을 압축 해제 후,
   KRPatch 폴더 및 DARKINST.cfg, cam_mod.ini를 씨프2 설치 경로에 넣는다.
   * DARKINST.cfg, cam_mod.ini는 덮어씌워질 것이기 때문에,
     원본 파일 백업 권장

3. 씨프2를 플레이한다.
   * 그래픽향상 EP2 모드를 적용 시,
      EP2용 한글 간판 및 버튼 텍스쳐의 추가 적용이 필요합니다.
      - 'EP2용 한글 텍스쳐' 폴더에서 KRPatch 폴더의 mesh.crf, obj.crf을 복사 후,
        기존 KRPatch 폴더 안의 파일을 대체하시면 됩니다.
        cam_mod.ini는 씨프2가 설치된 폴더의 파일을 대체하시면 됩니다.
        (mod_path 설정을 잘 아시는 분은 cam_mod.ini를 대체하지 않으셔도 됩니다.)

+) 씨프2의 기본 조작키 설정은 제법 현대화되어있으나,
    기본 이동키에서 달리기(Shift키)는 따로 눌러줘야 작동하게 되어있습니다.
    편의상 키설정(기본 걷기 -> 달리기로 변경)이 필요하여,
    제가 개인적으로 쓰는 키 설정을 SAVES 폴더로 동봉했습니다.
    SAVES 폴더를 씨프2 설치 경로에 덮으시면 됩니다.

    게임 내에서 "설정" - "조작 설정..." - "불러오기"
    "Zero-bangsong Bindings"를 불러오시면 됩니다.

    WSAD 기본 이동키, Q/E 옆으로 기울이기, F 앞으로 기울이기, G 나침반
    X 앉기, Z 앞으로 걷기, Shift 살금살금 움직이기, V 막기, 휠버튼 아이템 치우기

    * 소리나는 타일 등 걸어다니실때 Shift + Z 키로 움직이시면 편리합니다.
      앞으로 걷기 키를 일정 간격으로 반복하시는게(발소리 내기 전까지만 이동 반복)
      제일 베스트 방법이긴 합니다.


===============
문제 발생 시 확인사항
===============

Q1. 한글이 안 나와요!
     A1. DARKINST.cfg 내 language korean+english 가 기입되어 있는지 확인하세요.
          cam_mod.ini 내 uber_mod_path OSM+KRPatch 가 기입되어 있는지 확인하세요.

Q2. 영상에서 한글 자막이 안 보여요!
     A2. DARKINST.cfg에 movie_path .\KRPatch\MOVIES 가 기입되어 있는지 확인하세요.

Q3. 인게임 인터페이스가 너무 커요!
     A3. DARKINST.cfg 내 d3d_disp_scaled_2d_overlay 64를 삭제하세요.
          (게임 해상도 설정에 따라 자막이 콩알만하게 보일 수 있습니다.)

Q4. 옵션에서 조작키 설정 중에 깨진 글자가 화면을 덮어요!
     A4. 한글폰트가 부족해서 발생하는 문제이며, 현재로서는 엔진 한계상 해결 방법이 없습니다..
          키 설정하시는 데 크게 지장은 없으실 것이기 때문에 그대로 하시면 됩니다.


===============
참고사항
===============
ㅇ  현재 경비병의 반응 대사 등은 의도적으로 자막 숨김되어있습니다.
     (중요한 대사를 가리게 되거나, 긴장감 감소 등)

   - 경비병들이 뭐라고 하는지 궁금하신 분들은 KRPatch 폴더 내 USER.CFG를 메모장으로 여시고
      subtitles_hide_types fx+bark+urgent  에서 bark랑 urgent를 삭제하시면 됩니다.

      * 일부 미션에서는 극도로 정신사납게 만들기 때문에...
        한번 클리어 하시고 하시기를 권장드립니다.
