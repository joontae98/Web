# JavaScript

 객체 기반의 스크립트 프로그래밍 언어   
 JavaScript는 웹 브라우저 내에서 주로 사용하며, 다른 응용 프로그램의 내장 객체에도 접근할 수 있는 기능을 가지고 있다.
 ***
* CamelCase  -  단어가 합쳐진 부분마다 맨 처음 글자를 대문자로 표기하는 방법
* array
  * push() - 배열의 끝에 요소 추가
  * unshift() - 배열의 앞에 요소 추가
  * pop() - 배열의 마지막 요소 추출
  * shift() - 배열의 첫 요소 추출
  * indexOf() - 배열의 요소가 없으면 -1 리턴 있으면 인덱스 값 리턴
* 객체
  
  	  var mydog = {
		    "a hat": "ballcap",
		    "shirt": "jersey",
		    "shoes": "cleats"
	    };
   
 객체의 이름에 공백이 있는 경우 대괄호 표기법 사용

	mydog["a hat"];
 
 대괄호 안에 변수 입력가능 하고 동적으로 수집 가능

    var a = "a hat"	   
    mydog[a];
  
  새로운 속성을 추가 삭제(delete) 변경 가능
 
    delete mydog["a hat"];
    
  객체에 속성이 있는지 확인하는 메서드   
  
    mydog.hasOwnProperty("a hat")
