[Deployment]
Vercel URL: https://ossassignment23.vercel.app/

[Key Learning]
- 자바스크립트에서 배열을 이용해 간단한 데이터베이스를 구현하고 관리하는 법
- 각종 함수를 정의하고 불러오는 법
- 자바스크립트에서 객체를 생성하고 인자로 넘기거나 배열에 추가하는 등 객체 관리
- 
[CRUD Service]
주제: 가상 RPG 게임 캐릭터 관리
데이터 Fields
- num: 캐릭터 번호
- nickname: 닉네임
- class: 클래스(직업)
- level: 레벨
- attack: 공격력
- defense; 수비력
- speed: 스피드

Create / Read / Update / Delete 구현 방법
- Create: Form에서 입력받은 캐릭터 정보로 객체를 생성하고 chracters 배열에 push()하여 새로운 캐릭터 추가
- Read: characters 배열의 데이터를 forEach()로 각각 조회하며 renderCharacters() 함수를 통해 화면에 출력
- Update: 수정 버튼을 클릭하면 해당 캐릭터의 정보를 editCharacter()을 이용하여 Form에 불러온 후 수정된 데이터를 배열에 반영.
          이 때, editIndex를 이용하여 새로운 캐릭터 생성인지 기존 캐릭터 수정인지 구분.
- Delete: 삭제 버튼을 이용하면 find()와 indexOf()를 이용해 삭제할 캐릭터를 찾고 splice()를 이용해 배열에서 삭제

[JavaScript]
- querySelector(): 원하는 요소 검색 및 사용
- getElementById(): 원하는 요소를 ID를 이용해 검색 및 사용
- addEventListener(): form의 submit 이벤트를 감지해 캐릭터 생성 및 수정 기능 실행
- createElement(): 캐릭터 정보를 출력할 테이블 열(tr)을 동적으로 생성
- appendChild(): 생성한 <tr>을 <tody>에 추가
- Array: 여러 캐릭터 데이터를 객체 형태로 저장하고 관리
- forEach(): characters 배열의 각 요소를 순차적으로 선택
- find(): index를 기준으로 배열에서 특정 요소 선택
- indexOf(): 배열에서 특정 요소의 위치를 확인
- splice(): 배열에서 선택한 캐릭터 삭제

[AI / Search Usage]
ChatGPT 
- Table의 요소로써 버튼을 넣는 방법 질문 -> <td></td>로 <button>을 감싸기
- push(), find(), splice() 함수 사용법 질문 
- 백틱 `` 사용법 질문 -> 문자열을 ``으로 감싼 후 안에 ${}을 넣어 문자열 안에서 변수를 출력하기
- form label의 길이 다름으로 인한 정렬 방법 질문

[Problem&Solution]
함수를 여러 개 사용하다보니 디버깅 과정에서 어떤 함수에서 문제가 발생했는지 알기가 힘들었다. 
console.log() 기능을 이용하여 각 단계별로 console에 출력되게 하여 문제를 해결했다. 

[Reflection]
저번 CRUD service 구현 과제 당시에는 모든 기능을 하드 코딩하여 껍데기는 만들었지만 실제로는 전혀 작동하지 않는 서비스였기에 아쉬움이 남았었는데,
본 과제에서는 배열을 이용하여 간단한 데이터베이스를 구축하고 해당 데이터베이스를 실제로 활용할 수 있는 과제였기에 한층 더 흥미로웠다. 
또한 백엔드 없이 프론트엔드만을 가지고도 이 정도의 기능은 구축할 수 있다는 점을 느끼게 되었다. 

