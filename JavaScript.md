# JavaScript

 객체 기반의 스크립트 프로그래밍 언어   
 JavaScript는 웹 브라우저 내에서 주로 사용하며, 다른 응용 프로그램의 내장 객체에도 접근할 수 있는 기능을 가지고 있다.
 ***
* let, const 변수 
	- let 변수는 재할당이 가능, const 변수는 재할당 불가능
	- const 변수는 변수명을 대문자로 작성
	- 기본적으로 변수는 const를 사용하고 재할당이 필요한 경우 let사용   
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
   
	 * 객체의 이름에 공백이 있는 경우 대괄호 표기법 사용

			mydog["a hat"];

	 * 대괄호 안에 변수 입력가능 하고 동적으로 수집 가능

	   	   var a = "a hat"	   
	    	   mydog[a];

	 * 새로운 속성을 추가 삭제(delete) 변경 가능

	    	delete mydog["a hat"];

	 * 객체에 속성이 있는지 확인하는 메서드   

	   	   mydog.hasOwnProperty("a hat")
* Math 클래스
  * 0 ~ 1 사이의 난수 생성 = Math.random()
  * 가장 가까운 정수로 내림 = Math.floor()  
  * 0 ~ 9 사이의 정수 생성 = Math.floor(10*Math.random())
  * x ~ y 사이의 정수 생성 = Math.floor((Math.random()*(y-x+1))+x)
* 비동기 Promise

		const request = new Promise((resolve, reject) => {
			if(조건) {
				resolve(); //전송이 성공했을 경우
			} else {
				reject(); //실패 했을 경우
			}
		})

		request.then(result => { }); //resolve가 실행된 후 실행
		request.catch(error => { }); //reject가 실행된 후 실행 
