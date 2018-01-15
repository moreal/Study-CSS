# Transition

## Transition 이란
element의 property 가 변경될때 그 변경 과정을 부드럽게 꾸며주는(?) 기능이다.  
렌더링 엔진에서 다루는 듯 하고 엔진에 따라 다르게 설정해 줄 필요가 있는 듯하다.

## Detail
transition-property : width , height 같은 것을 지칭한다.

transition-duration : 지속되는 시간을 말한다. : 이 값이 작을 수록 빠른 애니메이션이 실행된다.

transition-timing-function : 시간을 어떻게 할지에 대한 설정이다. (세세한 설정) : AE의 곡선 처리를 보아도 괜찮을 것 같다.

transition-delay : 해당 트랜지션이 실행되기 전의 지연시간을 지정가능하다

```CSS

box1 {
    transition-delay: 1s;
}

box2 {
    transition-delay: 2s;
}

box3 {
    transition-delay: 3s;
}

```

### 시간단위

s : 초

### transition-timing-function : Detail

ease, linear, ease-in, ease-out, ease-in-out, cubic-bezier, step-end, step

ease : 처음에 빠르고 중간에 느리다가 다시 빨라진다.  
linear : 계속 동일한 속도로 이동한다.  
ease-in : 시작할 때 느리다.  
ease-out : 끝날 때 느리다.  
ease-in-out : 시작과 끝에 늘리다.  
cubic-bezier : 자신이 원하는 대로 함수를 커스텀 한다.  
step(n, end) : n 번에 걸쳐 변화합니다.  
step-end : 중간과정 없이 duration 시간이 흐른 뒤 종료한다.

cubic-bezier 함수만들기 (http://cubic-bezier.com/#.15,.46,.78,.15)

## 트랜지션 완료 후 처리

```javascript
element.addEventListener("transitionend", function, true);
```

이런 함수로 트랜지션이 끝날을 때의 처리를 해 줄 수 있다.

## 브라우저 별 호환성을 위한 처리

chrome,safari : -webkit-
Firefox : -moz-
Opera : -o-