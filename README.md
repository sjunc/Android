# Android
linux kernel os
HAL 가상머신
JVM = ART(안드로이드 런타임) 
프레임워크 
app -> 코딩
 
공통구조 

API 함수모음
Application Programming Interface
5.0이상 api 21 롤리팝 이상 98%

c
#include <stdio.h>(선행처리기 preprosser)

main()
int i=3;
int j=4;
int k=0;
K=sum(i,j);
print k;
int sum
...
작성하면 함수를 썼다가 다시 돌아옴: 절차형

클래스형 c++, java 코틀린의 해당
class book
....
변수와 함수가 한 세트로 쓰임. 객체지향에 맞게 클래스형으로 코드를 짜야함.

 
int i                               변환(컴파일러)
print -> 인간이 쓰는 고급언어      -->     기계어(저급언어)
sum                                         

어셈블리어

00101            ->  ADD                         다시 2진수로
01110            ->  Print 연상기호 mnemonic   -> 
11010            -> sum                            어셈블러

basic 인터프리터 

한줄씩 번역하는 형태

JAVA
Hello. java javac hello.java -> Hello.class =>실행 " java hello"

                             컴파일러    인터프리터(한 줄씩 실행함)
C
소스코딩 .c -> .obj 오브젝트 파일 -> .exe 실행파일

             컴파일      (함수를) Linker, (메모리에) Loader

안드로이드
 코틀린 -> 바이트 코드 -> .apk 실행파일
interface definition language AIDL

코루틴
프로세서 processor(CPU) 1프로세스 1task 는 비효율
고로 프로세스를 쪼개기 -> 스레드 tread 
모바일 환경에서 하드웨어 성능 문제로 스레드를 더 잘게 쪼갤 필요성이 생겨서 더 잘게 쪼겜

에뮬레이터를 제공한다. 
program 경로 작성할때 공백, 한글, 특수문자() 주의해서 작성

Software Development Kit SDK

앱과 gradle scripts 

과제: 제출하진 않아도 되지만 하고 와라. 
안드로이드 스튜디오 설치하기
67p까지 에뮬레이터까지 실행해보고 오기. 

----------------------------------------------------
컴퓨터 꺼져서 날라감 3주차

75p 
package name 소문자로만 작성할 것
example 명을 사용하지마라
 76p
mainactivity.kt 소스파일 kotlin = kt
res-layout activity_main.xml 보여지는 면 
kotiln 위치 - java
임포트하라거나 빌드피겨를 해라를 만들라고 하면 해야함.

레이아웃편집하기
색변경 
81p 회전
hello world를 hello kotlin 으로
83p 레이아웃 편집 view binding  방식
build.gradle.kts

항상 작성할 테니 외울 것

   buildFeatures{ 
        viewBinding = true
    }

85p 
이름은 소문자-> 대문자를 섞어서

oncreate 함수 위와 layout 사잉에 

ActivityMain  입력시 뒤와 import 자동 생성 

1.싱크
3장 96 empty view activity로 선택
로그 활용방법
v verbose 말이 많은
I information
d debug *많이 쓰임*
w warnig 
e error *많이 쓰임2*


과제 hello kotlin 코딩 과정 이유와 결과 간단히 작성후 과정

cyron@naver.com
---------------------------------------------------------------------
4주차

반드시 싱크를 맞춰라.
target 
compile 
sdk 버전을 34로 맞출것. 
system.out("here1")를 중간 중간 찍어서 어디부터 문제가 생긴지 알 수 있음. 
log를 찍어서 알아보기
오늘은 필수적인 이론

작성 규칙 coding convention 

var variable int i = 3;
            (class) 변수 상수 

c나 자바와 달리 str을 var로 가능
Int Float - 4byte 자료형만 봐도 됨
float 浮(뜨다)動소수점 
Double과 구별하기 위해 끝에 대문자 F를 붙임.
_ under score
Long int 8byte 버전 구별을 위해 뒤에 대문자 L을 붙여준다.

Char 'A' <> int 65 ASCII c와 자바에서 상호호완 가능
String"여러 개의 글자이고 쌍따옴표"

정수와 실수는 다른 타입이기 때문에 casting 데이터 타입 변형을 거쳐 변환해야한다. 
Double int type을 지정해주지 않았을 때의 기본값
음수 표현방법
1의 보수 one's complement 011 -> 100     3, -3
2의 보수 two's complement 011 -> 100 -> 101 2의 보수 = 1의보수 + 1 3, -3, -3 
앞에 $를 넣으면 코드로 인식, 앞뒤 공백 필요
var 
val 읽기전용 변수 상수랑 비슷함
const 상수 
const int Max;
int = 10              ( X )

const int Max = 10;    ( O )
Max = 11 X
한번에 선언해야 함

coding convention 
class는 대문자-소문자로 써준다.
metod (클래스에서의 함수), 변수명, 함수명  소문자-대문자
상수 모두 대문자로 작성

조건문 
if - boolean(True False) 으로 결과가 나옴

==
!= , <>
&&  and
|| or
! 부정
   
Xor 베타


기본코드 
12line 부터 코딩
5라인에 import ardroid.util.Log를 넣어줘야 책의 실습가능


when(파라미터)  다른 문법 switch 
조건-> {
 실행 }
조건2

else default 
{ 실행 }

, 를 통해 조건을 설정하거나 범위로 설정 가능함. 
파라미터도 생략가능 
비교 if                     막연한 비교
여러가지를 동시에 when  범주 비교

모바일 환경이기에 간결해지기 위해 등장

107 1번
117, 118 2번
120 3번
121 4번
122 5번
124 6번 
125 7번
126 8번 9번 
코딩을 작성한 후 결과 출력 

---------------------------------------------------------------------------------------------------------------------
5주차 
중간고사 범위 4장까지 
배열(Array)과 컬렉션(Collection)
사상: 왜 쓰는지 -> 배열: 하나하나 보내지 말고 묶어서 한번에 보냄. 용량은 같아도 효율적임

배열
개수를 정해놓고 사용. 개수를 중간에 추가나 제거 불가
var 변수 = 자료형Array(개수)
string 없음. 그 자체로 배열 var stringArray = Array(10, {item->""})
index 첨자 0부터 시작
배열명[인덱스] = 값   배열명.set(인덱스, 값) 
get 빼기 set 넣기
*넘어갔을 때 나오는 배열 에러는 외워라 IndexOutOfBoundsException: 자주 나옴

컬렉션(동적 배열)
코틀린에만 있음 
리스트, 맵*(딴 곳에서 많이 씀), 셋
처음 크기를 고정하지 않고 임의의 개수를 담을 수 있음
시험에 나오니 외울 것

리스트(List) 
중복 입력 가능, mutable
var mutable <> val immutable
.add를 써서 추가 순서대로 인덱스가 저장됨
.get을 써서 값을 꺼냄
.set을 써서 값을 수정함
.removeAt을 써서 인덱스를 제거 , 뒤의 값이 땡겨옴
.size 프로퍼티 괄호 없음  컬랙션 개수를 가지고 옴
 
셋(Set) 
중복을 허용하지 않음. index로 조회 안되고 get 지원 안 함
셋 사용 전체를 출력
.remove 셋 값으로 조회해서 삭제 중복불가해서 값이 고유값임. 
.add 

맵(Map) 파이썬 딕셔너리랑 비슷 
key와 value 키와 값
.put 으로 넣음
.get으로 사용
.put으로 수정
.remove로 삭제 다른 값들의 인덱스가 변경되지 않음.

imuutable collection
사용만 가능 불변형이기 때문에

반복문 
for 
for (var in  .. 
for (var시작 until 종료값)
for (var in 시작값..종료값 step 단계) 단계로 건너뛰기
for downTo  큰 수에서 작은 수 감소시키기

while 조건식이 참일때 
while은 범위를 적지않기 때문에 증감시키는 코드를 넣어줄것
do while 일단은 1번은 함. while이 False 여도

반복문 제어
break 반복문 탈출 쓰지 말라고 함 continue, goto
continue 중단하고 다음 반복문


예제 4번 결과가 6까지 출력한다는 점과 5번에서 얼마나 건너띄는지 주의
실무에서 반복문은 중첩(nested)은 2개가 주 
면 행 렬 3개 2개 1개 중첩 반복문

함수
C
#include <stdio.h>
main(){
int i = 3
int j = 4
int k = sum(j,i)
printf k;
}\
int sum (int a, int b)
int c = 0;
c= a+b;
return c;

코틀린 함수
fun 함수명(파라미터명:타입): 반환 타입 {
return값
}
파라미터는 immutable 
7, 8 비교
Area(int i)
Area(int i, float a)
Area(int i, float a, int K);
Area(2)
Area(2, 3.0)
Area(2, 3.0, 4)

이런 방식을 overloading이라고 함

 

6개
134 10
140 11
142 12
145 13 
152 14
157 15
165 16




-------------------------------------------------------------------------------------------------------------------------------------------
6주차

~299p 까지 시험
c는 필요하면 써내려 가지만 자바나 코틀린 같은 객체지향은 모아서 작성한다.
클래스 
변수와 함수(메서드)의 모음이다.

class 클래스명 {
클래스 스코프
}
클래스를 사용하기 위해서 생성자 constructor가 호출되어야 한다. 2개를 준다.
프라이머리 헤더, 세컨더리 

프라이머리 
유형 1 constructor를 쓰기 V

유형 2 constructor만 생략(parameter)

유형 3 init으로 초기화

유형 4 init 대신 val 

세컨더리 

유형 5 유형 3에서 init 자리에 들어감. V

파라미터의 개수, 또는 타입이 다르면 여러 개를 중복할 수 있다.*** overloading

유형 6 default

클래스의 사용
클래스명()
인스턴스 같은 클래스를 여러 개

유형 7
var one = Person("value")
// 또는
var two = Person(1004)

클래스 내의 변수 속 맴버 변수(프로퍼티), 멤버 함수(메서드)

encapsulation 컴퓨터는 클래스 안의 내용을 알 수 없다.
그래서 인스턴스에 점을 붙여서 안으로 들어간다. 
pig.프로퍼티 = 'piggy'
pig.메서드()

바로 클래스로 호출하는 법 object 별로 안 좋음
object 클래스명
앱 전체에서 딱 한번만

companion object
오브젝트처럼 사용가능하게 한다. {} 안에 있는 기능만 그렇게 하게 한다.
*코틀린만의 문법* 밖의 기능은 똑같이 인스턴스를 만든 후에 .을 써서 똑같이 사용한다.

데이터 클래스
data class 클래스명 (val parameter1: type, var parameter2: type)
굳이 구별 시킨 이유 1. 네트워크로 데이터를 주고 받을 때 2. 로컬 앱의 데이터베이스를 다루기 위해 

상속과 확장

open class 부모
오픈부터 해주기 

class 자식 클래스: 부모 클래스() 
상속하기

생성자 파라미터가 있는 경우 상속

세컨더리 생성자만 있을 땐 클래스 다음 괄호 생략


오버로딩 overroading 파라미터의 타입과 개수를 다르게 정의
오버라이딩 overriding 재정의

상속받고 재정의 
동일한 이름의 메서드나 프로퍼티를 사용할 필요가 있을 경우에
메서드 오버라이드도 open을 붙여줘야 가능
프로퍼티 오버라이드 ==

익스텐션
fun 클래스. 확장할 메서드(){
//코드 
}
.plus를 활용해 익스텐션 가능 

설계 도구

패키지
계층 구조로 되어있음

추상화
abstract 껍데기만 먼저 만들기 뭘만들지 파악 

인터페이스
기능이 없이 메서드만 나열
interface 인터페이스 명{
var 변수: String
fun 메서드1()
fun 메서드2()
}
추상화의 일종

접근 제한자
클래스 안의 멤버를 접근하는 방법 인터페이스, 메서도, 프로퍼티도 가능

제네릭
입력되는 값의 타입을 자유롭게 사용하기 위한 설계


프로텍티드랑 프라이빗 부모클래스 직접 호출 가능한지 해보기 get, set을 통해 접근해야함.

183 17 
193 18

215p~ 실습


--------------------------------------------------------------------------

7주차 OOP object oriented(지향)
override 부모의 메서드 재지정
overload 서로 다른 자료형들을 불러옴

4장 299p 
null 값
항상 이슈의 중심. 오류가 많이 나고 프로그램이 다운됨. 의도에 상관없이 프로세스 상 만들어질 수 있음
처리
그냥 모두 허용할 수 없음-> 비번, 주민번호 등
 
var variable: type? = null 허용
함수에서 null 허용을 할 땐 ?를 쓰는데 웬만하면 null일 때와 아닐때를 구분해줘라(안정성 향상)
리턴 타입에도 물음표를 붙여 null값을 반환 가능하다.
safe call ?.   ?(null).(if)
간단하게, if 로 아닐때 구분했던 걸 . 으로 그냥 대체 인자?.메서드   인자가 null이면 프로퍼티가 아닌 null반환, 아니면 프로퍼티
elvis operator
?: Null일 경우 갖게 되는 기본 반환값 설정

지연초기화
기존의 선언->초기화 가 아닌 내가 필요할 때(호출할 때)만 초기화 하겠다. 선언-> 필요할때 -> 초기화 모바일 특성 메모리 낭비 
lateinit var    /     lazy val    초기화를 꼭 함께 작성할 것, 둘 다 조건이 많이 붙음

스코프함수 (개념만)
영역(스코프)안에서 it이나 this로 , 코드 축약. run, let, apply, also, with 예약어

this run, apply, with this는 생략가능
it  let, also it 생략 불가능

4장
레이아웃
파일은 .xml 파일이다.
activity_main.xml res-layout-.xml에 위치 (MainActivity.kt java 아래 있음, 클래스 개념이라 대문자가 섞인 걸 알 수있음. 레이아웃 파일이 모두 소문자 인것과 대비됨)
컨스트레인트 레이아웃 2주차 했던 기본
constraint 제약조건

선택 영역 핸들러
선 컨스트레인트
오른쪽 편집기

랩 컨텐트 내용물 크기에 맞춰서 포장
픽스드 박스 고정
매치 시작과 끝에 맞춰서 크기조절

매치로 하고 위 세모 클릭 ratio 가로: 세로 비율 설정

툴바
없으면 팔레트 레이아웃 항목

체인으로 연결
여러개의 레이아웃을 겹쳐라. 

가이드라인 
팔레트 헬퍼 

리니어 레이아웃 Linerlayout**

레이아웃을 겹치거나 기본을 변경시킬 수 있음

gravity 정렬

scrollview layout

frame layout 
위젯 중첩해서 사용할 때, 처리 속도가 가장 빠름.

xml 
html과 달리 주어진 태그뿐만이 아니라 만들수 있음. 

res
부분에서 보이는 부분 편집
RGB

FF000000 2자리 수 씩 16진수 표현

264 이미지
273 체크박스
280 로딩
283 시크바 음량
288 별점

소스 코드 텍스트로 제출
결과 캡쳐 후 이미지로 제출
---------------------------------

## 기말까지의 범위 
-----------------------------------------------------
5장 (이론)

액티비티: 사용자가 직접 보고 입력하는 화면을 담당
.kt 액티비티 .xml 레이아웃
컴포넌트 핵심 요소
컨텍스트context(작업 공간, 클래스의 집합)
컨텍스트의 모음, 큰 통 컨테이너 container

1. application context     2. base context(activity, service, content provider, broadcast receiver)

인텐트 intent(의도) java vo bto bin
사이 연결

스킵

6장 443p

권한  *모바일 중요 (보안)*

spec (명세)
권한 명세			기능 명세
(사용 여부) 		(기능이 있는 경우만 사용)

app - manifest 폴더 밑	자동으로 추가됨 
ArodroidManifest.xml	수동으로 넣는 경우도 존재
<uses-permisson /> 태그	<uses-feature />
			기능이 없으면 스토어에서 앱이 검색 안되게 하게 함
			requied를 false로 하면 기능이 없어도 검색 가능(오류가 날 것이기에 예외처리)

		권한 
1. 일반 권한 		
설치 시 팝업 버전마다 다름
<uses-permisson />

2.위험 권한 
개인정보 처리
권한 명세하고 소스 코드에 권한 요청 및 처리를 따로 작성해야함

3.서명 권한
한번 인증하면 인증 안함. 일부 서명권한은 써드파티(3rd-party) 앱에서 사용 불가

권한은 그룹으로 구성
그룹으로 묶인 권한은 한번에 처리

위험한 권한 처리
1.AndroidManifest.xml 정의
2. 코드 구현

url 위치(location): naver.com
uri 특정(identify) 리소스 하나 네이버 로고 이미지 하나

package com.example.permisson

import android.Manifest
import androidx.appcompat.app.AppCompatActivity
import android.os.Bundle
import android.view.LayoutInflater
import android.widget.Toast
import androidx.activity.result.ActivityResultLauncher
import androidx.activity.result.contract.ActivityResultContracts
import com.example.permisson.databinding.ActivityMainBinding



class MainActivity : AppCompatActivity() {

    val binding by lazy { ActivityMainBinding.inflate(LayoutInflater)}

    lateinit var activityResult:ActivityResultLauncher<String>

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(binding.root)

        activityResult = registerForActivityResult(ActivityResultContracts.RequestPermission()){
            isGranted ->
            if (isGranted){
                startProcess()
            }else{
                finish()
            }
        }
        binding.btncamera.setOnClickListener {
            activityResult.launch(Manifest.permission.CAMERA)
        }
    }
    fun startProcess() {
        Toast.makeText(this, "카메라를 실행합니다.", Toast.LENGTH_LONG).show()
    }
}
-----------
10주차

파일 입출력
정보 -파일(잘 안씀, 엑셀과 같이 저장된 경우) 모바일은 용량, 메모리 때문에 주로 이 방식을 선택함
    |_  DB

기계에 저장: 입력
나가는 거: 출력

안드로이드는 리눅스 위에 가상 머신이 동작하는 플랫폼

특정 앱의 사용자가 접근할 수 있는 영역 내부 저장소 internal storage (line, kakao 따로따로)
모든 앱이 공용으로 사용할 수 있는 영역 외부 저장소 external storage (ex.gallery)

외부 저장소는 manifest 권한을 명세 해야함.


파일 사용하기

1번
먼저 File 클래스 생성
생성자 부르기 File("경로")
저장 val file = File("경로")

2번
filesDir 프로퍼티 사용
val file = File(baseContext.fileDir, "파일명")
액티비티의 경우 fileDir이 기본 프로퍼티다. 
val file = File(filesDir, "파일명")

사용하기에 앞서 있는지 체크하고 없는 경우 예외처리가 필요하다.
.exists 존재여부 isFile 경로가 파일인지? isDirectory 경로가 디렉토리인지? name 이름 반환 createNewFile() 새 파일 mkdirs 디렉토리 생성 delete() 삭제 absoulePath 절대 경로 반환(경로 전부) 
디렉토리 만드는 명령어 linux mkdir(안드로이드도 이 방식을 따름) / dos md(과거) . 자기 자신 .. 한칸위 (상대경로)

스트림 stream
읽고 쓰기 위해 파이프를 연결(읽고 쓸 때만)
open하고 close를 해서 메모리 누수를 방지

입력 stream	 출력 stream
InputStream 	OutputStream
텍스트냐 아니냐를 구분(stream으로 끝나냐 read, write로 끝나냐)
read  		write

모양을 알것

텍스트 파일 읽기
package com.example.fileio

import java.io.BufferedReader
import java.io.FileReader

class FileUtil {       // 클래스 FileUtil을 생성
    fun readTextFile(fullPath: String): String{                       	// readTextFile이란 함수 정의 fullPath란 인자를 받으며 type은 string임
        val file = File(fullPath)					// file 이란 변수(상수같음)을 File에서 가져옴? 인스턴스? File은 임포트로 가져온 건가?
        if (!file.exists()) return ""				// 파일안에 프로퍼티를 사용. exists는 존재여부를 확인하므로 없으면 ""을 반환

        val reader = FileReader(file)				// 이것도 인스턴스? 일단 위에서 FileReader는 임포트 해옴 
        val buffer = BufferedReader(reader)			// == 
        var temp = ""					// temp란 변수 선언
        val result = StringBuffer()				// result란 상수적 변수 선언, 어디에서 온 값이랑 같은거지?
        while(true){						// 반복문이 true일 때
            temp = buffer.readLine()				// temp는 뭐 이렇게 됨.
            if(temp == null)break;				// temp가 비어있는 게 맞으면 멈춤
            else result.append(buffer)				// 아니면 result 속 append를 실행시킴. 
        }
        buffer.close( )					// buffer를 닫음
        return result.toString()					// 반환 result의 toString() 실행?
    }
   fun writeTextFile(directory: String, filename: String, content: String){
        val dir = File(directory)
        if(!dir.exists()){
            dir.mkdirs()
        }
        val writer = FileWriter(directory + "/" + filename)
        val buffer = BufferedWriter(writer)
        buffer.write(content)
        buffer.close()
    }
}
자바와 c에서도 이런 방식으로 구현 됨. 잘 기억해 둘것
class에 정의만 나와있고 
예외 처리와 출력은 어떻게 하는지 는 없는데 소스를 올려둘것

SharedPreferences (끝 s 주의) 공유참조
공용 데이터 저장소

저장 putString()  저장소   getString() 사용

키 값 쌍 (맵, 딕셔너리)으로 저장한다.

CRUD
create
retrive(read) 
update
delete

read가 아니면(put이면) apply를 마지막에 해줘라.
get(read)는 그럴 필요가 없다. 

getSharedPreferences( 이름, 모드)로 가져온다.

하나만 있으면
getPreferences(모드) 도 가능하다. 

데이터 저장과 불러오기는
editor 로 한다.

put 넣기
string (key) 쭉 쓰고 값을 쭉 넣는다.
apply 해준다.

get 가져오기
get자료형(key: String, defaultValue: 자료형)

삭제
remove 키의 값 삭제
clear 모든 데이터 삭제
이것도 apply 해줘야한다. 

apply 비동기적 저장 asyncronous
commit 동기적 저장 syncronous(보내고 받고)   db에서 마지막에 수정후 저장 할때 넣는다. 잘못 보냈으면 rollback() 해준다.

의존성 주입(추가)
특정라이브러리가 잇어야 동작하기에 dependency를 추가함. 
요즘은 자동이여서  딱히 필요 없다. 잘못 넣으면 버전이 안 맞아서 확인하고(developer.android.com/jetpack/androidx/releases/preference) 넣어주자. 




-----------------------------------------------------------------------------------------------------------------------------------------------------------

11주차
데이터베이스

코드와 정보는 모두 데이터베이스에 들어감.
파일로는 너무 많아서 데이터베이스는 필수적

ID table   ID 이름, 성별, 나이 등 table

			primary key							빅데이터						순간적으로 데이터가 몰리는 경우(수강신청, 명절 기차예약등)
두 테이블은 연결 되어있어 있음. pk끼리 연결 이런 DB를 RDB Relation DataBase         <----->         NoSQLDB (no는 약자임) archive(두고 쌓아두는 경우)		in-memoryDB - SSD					클라우드(가상화) 큰 서버에서 빌려씀
일반적인 데이터 베이스, 관계형 데이터베이스								대용량							속도						편리성, 보안 취약(관리자 귀찮음)


2차원 배열
column컬럼(필드)  row로우(레코드, 튜플)
SQL( Structured Query Language)
정의 DDL(data definition lang)               조작(DML)manipulation		 제어(DCL) control
테이블의 속성 바꾸기                             데이터를 CRUD		 데이터 권한 
만들고			     
삭제
수정

android는 SQLite를 경량으로 사용
db 연결은 중요함.

프로그래밍에서 파일 입출력과 db연결은 꼭 알아두자.

-----------------------------------------------------
12주차

기본 사항

file 입출력, DB 입출력
read	   SQLite
write

CRUD
Create
read - select  read만 성격이 다름
Update
Delete

Room
SQL 확장판 더 구조적으로 이루어져있음. (object화)
결과는 같다.

ORM(Object Relational Mapping) 자동 변환
쿼리를 건너뛰고 매핑으로 집어넣기.

kapt = java @(annotation) 명령어 

9장 
책이랑 많이 다름. 
카메라 사용 개인정보
권한이 있어야 사용 가능. 카메라(위험권한 445p)

뷰 바인딩 디펜던시 유지
xml 화면 만들기

-------------------------------------
스레드와 코루틴

스레드

컴퓨터
cpu
프로세스
덩치가 커서 조각내논 것: 쓰레드 thread

모바일
쓰레드도 크다. 조각(논리)내논 것: 코루틴 coroutine co 함께
동시성 프로그래밍 개념

stack 스택 lifo            queue 큐 fifo
top = bottom 문구
아무것도 없다는 뜻

--------------------------------------------------------------
기말 쓰레드 (타이머)
구글 지도 전까지 5장 ~ 10장까지
파이어베이스 코틀린 앱 개발 서비스
중간과 동일 방식




