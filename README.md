# introduction

제가 만든 일본어 JLPT 단어장을 소개합니다.
자료는 인터넷에서 JLPT 필수 단어를 찾고 직접 편집 및 작성하여 만들었습니다.
디자인은 현직 디자이너에게 의뢰하였으며 건네받은 모든 파일은 일러스트레이터로 제작되어 실제 구현은 100% 직접 했습니다.
기획부터 완성까지 약 10개월이 걸렸으나 실질적으로 개발에 들어간 시간은 전업으로 한다는 가정 하에 1개월 이하입니다.
프로토타입은 bloc패턴 및 hive로 제작되었으나 완성품은 getX로 리팩토링하여 만들었습니다.
실제 코드 및 사용된 패키지 정보가 필요하시다면 따로 요청해주세요.

![레벨선택페이지](https://user-images.githubusercontent.com/33222740/110444569-8964cd80-8100-11eb-81b7-e31a1a287cbf.gif)
메인페이지입니다. JLPT 급수를 선택할 수 있습니다. 선택된 아이템이 하이라이트 되도록 만들었습니다.


![뷰방식선택](https://user-images.githubusercontent.com/33222740/110444611-941f6280-8100-11eb-99da-5fd1ff56acca.gif)
챕터 선택 페이지입니다. 단어를 100개 또는 200개씩 볼 수 있도록 만들었습니다. 영상에 담진 못했지만 각각의 리스트는 고유한 키값을 가져 리스트의 위치를 기억합니다.


![스와이프](https://user-images.githubusercontent.com/33222740/110444674-a6999c00-8100-11eb-8659-837eed22ee10.gif)
하나의 챕터를 선택하면 단어장 화면이 나옵니다. 단어 카드를 왼쪽으로 스와이프하면 해당 단어를 아직 외우지 못했다는 의미로 현재 단어 리스트의 맨 뒤로 넘어가서 다시 볼 수 있습니다. 
오른쪽으로 스와이프하면 해당 단어를 다 외웠다는 의미로 다시 나오지 않습니다. 좌스와이프 시 앱바 하단의 숫자가 갱신되지 않지만 우스와이프 시 갱신되는 것으로 확인할 수 있습니다.
또한 화면 하단 버튼도 스와이프와 같은 역할을 합니다.


![목록이동](https://user-images.githubusercontent.com/33222740/110444704-af8a6d80-8100-11eb-85b3-cf0b2073128c.gif)
모든 단어를 다 외웠다면(우스와이프했다면) 다이얼로그 창이 뜨며 챕터 선택 페이지로 이동할 수 있습니다.
챕터 목록 우측에서 5개의 구슬 중 하나의 구슬이 분홍색으로 활성화되는 것을 확인할 수 있고 이 구슬 Row들은 해당 챕터를 몇 번 공부했는지 확인하는 용도로 쓰입니다.


![진행중아이콘](https://user-images.githubusercontent.com/33222740/110444787-c3ce6a80-8100-11eb-8840-222ea70f1809.gif)
선택된 챕터의 아이콘이 빨간색으로 변하기 때문에 나중에 봐도 해당 챕터를 공부하는 중인지 아닌지 확인 가능합니다. 
참고로 한번의 공부를 끝낸다면 아이콘은 다시 비활성화되며 이것은 이전 영상에서 확인할 수 있습니다.


https://user-images.githubusercontent.com/33222740/110444900-e6608380-8100-11eb-93b8-dbaac714a57c.mp4
앱을 완전히 종료시켰다가 다시 켜도 자료는 이전처럼 유지됩니다.

