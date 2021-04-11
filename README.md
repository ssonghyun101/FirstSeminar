# FirstSeminar
## 생명주기 사진
https://user-images.githubusercontent.com/81518783/114307035-d2051180-9b18-11eb-9d43-861707c97204.PNG

## 화면전환 후 데이터를 가져온 로직 정리
##### SignUpActivity
1. 아이디, 비밀번호에 입력된 값이 있는지 체크한다
2. 입력된 값이 있을 경우
3. 입력된 값을 String 값으로 받아준다
4. Intent를 통해 SignUpAcivity -> SignInActivity로 전환할 때 putExtra를 통해 String 값을 전달한다
5. SignInActivity로 이동
6. 액티비티 실행 시getData()함수 실행
#### GetData 함수 내용
6-1 intent를 받아온다
6-2. hasExtra를 통해 intent로 받아온 값이 null인지 아닌지 체크한 후
6-3. setText로 가져온 값을 띄워준다 


## 과제를 통해 성장한 내용

#### 아쉬운점
1. 일단 github 사용이 처음인지라 굉장히 많이 해맸다... 언제쯤 익숙해질련지 모르겠다
2. registerForActivityResult를 구현하지 못한 점
    2-1. 이유 : registerForActivityResult를 사용하려면 version을 바꿔야한다. version을 바꾸니 모든 binding에서 에러가 났다.
    2-2. 도저히 모든 binding의 에러를 고칠 염두가 나지 않았다.
3. 계속해서 system ui error가 났다. 평화오빠의 조언대로 모든 view의 ConstraintLayout의 start와 end 중 1, top과 bottom 중 1을 맞추었다. 애뮬을 돌리니 처음에는 error가 나지 않았다.
하지만 에러는 늦게 다시 발생했다. 이유를 모르겠다.


#### 잘한 점
1. 남이 잘한 코드를 보지않은 채 스스로 먼저 코드를 작성했다. 어려워도 의지하지않고 스스로 해보고 싶었다.
2. 미미하지만 도전해본 것

#### 앞으로 할 것
1. system ui error 원인 분석
2. registerForActivityResult 추가하기
3. Parcelable를 통해 한번에 여러 데이터를 전달해보기(intent를 검색하다가 알게되었다)
4. github 익숙해지기....ㅂㄷㅂㄷ
5. 코드리뷰보면서 잘하는 사람들은 어떻게하나 보고 따라하고 이해하기
