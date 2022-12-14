# 생활코딩 자바스크립트(23강~29강): 배열,반복문활용,함수개념~활용


## 1). 배열과 반복문 활용:

- 코딩에서 검색하는 법을 익히는 것이 중요하다.

- javascript get element by css selector multiple: element에서 어떤 태그를 전부 가져오는 법을 검색하는 법

- document.querySelectorAll( ): element에서 어떤 태그를 전부 가져오는 법

- 콘솔에서 밑에 줄로 한 칸 내리는 방법: Shift + Enter

- ```var alist = document.querySelectorAll('a');
   var i = 0;
   while(i < alist.length){
   alist[i].style.color = "powderblue";
   i = i + 1;}  : 변수를 그대로 작성한다.```

- 자바스크립트에서 index 표시는 무조건 작은 따옴표로 한다(큰 따옴표로 하면 오류가 발생함)

## 2). 함수:

- 함수 = 수납상자(코드가 많아질때 정리정돈하는 도구)

- 함수의 역할: 반복되고 복잡한 코드를 함수의 형태로 정리하여 간결하고 효율적인 코드로 바꿔줌

- 스크립트 태그 밑에 함수를 만들어서 작성
```
function two(){
 document.write('<li>2-1</li>');
 document.write('<li>2-2</li>');
 }
 ```

- parameter(매개변수): 입력
  argument:인자
  return; 출력

- 줄 바꿈 태그 : ```'<br>'```

- parameter 와 argument는 함수의 입력값과 관련된 것

ex). 
```
function sum(left,right){
document.write(left + right + '<br>');
}
sum(2,3)
``` 
함수의 틀에 해당하는 변수(left, right)가 매개변수, 함수에 넣은 변수(2,3)가 인자

- 표현식: 어떠한 결과 값을 도출해 내는 식

   ex). 1+1 =2 에서 1+1은 2에 대한 표현식이다.

- return은 함수의 출력값과 관련된 것 : return을 통해 출력하면, 다양한 용도로 사용가능하기에 기능성면에서 큰 이득을 준다. 

- 태그 안에 CSS(글자 색 바꿈)값을 주고 싶은 경우 : ```style = "color:red"```
ex).
```
    function sum(left, right) {
         return left + right;
     }
     document.write('<div style = "color:red">'+sum(5,7)+'</div>');
```

- 태그 안에서 CSS(글자 크기)값을 주고 싶은 경우: ```style = "font-size:*rem"```
ex).
```
    function sum(left, right) {
         return left + right;
     }
     document.write('<div style = "font-size: 3rem">'+sum(5,7)+'</div>');
```

- 각 태그가 괄호에 들어가면 ' ' 넣어주기

- ***함수를 만들때, 변수가 this로 묶여있으면, 함수의 매개변수를 self로 받고 바디 태그에서는 this로 표현한다!!!


## 3). 객체(object): 

```서로 연관된 함수나 변수를 그룹핑해서 정리정돈하는 것, 폴더와 비슷한 역할```

- 해당 함수들을 하나의 객체로 나타내어 보다 코드를 간편하게 만드는 작업이 필요
