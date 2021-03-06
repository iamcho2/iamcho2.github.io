---
layout: post
title: "아이디어 구체화 및 캐릭터 그리기" 
date: 2021-04-08
category: read 
excerpt: ""

---

# 아이디어 구체화 및 캐릭터 그리기

이걸 위해 아이패드를 샀다...! ^^

<img src="https://user-images.githubusercontent.com/28949235/114293062-f2f44500-9acd-11eb-8fd3-24a7195be619.jpeg" alt="IMG_5FBAFF419E8B-1" style="zoom:25%;" />

굿노트에 아이디어도 적어보고 조사한 자료들도 스크랩하고 뷰도 대충 그려봤다  
아주 편하고 좋더라고,,~~

![image](https://user-images.githubusercontent.com/28949235/114293103-57170900-9ace-11eb-836b-004748a78ee3.png)

앱 내에서 사용할 캐릭터들도 그려줬다.

### 기획 정리하기

정리해보자면, 이 앱은 **극지방에 사는 동물들이 지구 온난화 때문에 어떻게 변했는가!**  
를 통해 지구 온난화에 대한 경각심을 갖게 하고, 또 우리가 할 수 있는 일은 무엇인지 알려주는 앱이다.

각 Scene마다 코딩 요소를 조금씩 넣으려고 했다.

### Scene 1

요정(ㅋㅋ)이 날아와 WINTER LAND로 여행 갈 수 있도록 하는 boarding pass를 준다.  
캐릭터(나)에게 날개가 달리는 내용..!

비행기를 태울까 하다가 환경을 생각하자는 앱인데 ㅋㅋㅋ 비행기 태우는건 모순이라고 생각해서  
날개를 부여하는 방식으로...~

**코딩 교육적 요소** String  
boarding pass에 이름칸이 비어있고, string 변수를 바꿔서  
실시간 또는 `run my code`를 눌렀을 때 boarding pass에 넘겨준 String값이 들어간 뷰를 확인할 수 있다.

### Scene 2

WINTER LAND로 여행가는 내용!  
원래는 남극, 북극을 분리해 컨텐츠를 다룰 예정이었지만, 기획 구체화 도중 그냥 구분 없이 winter land로 합치기로 했다.  

함수 호출을 하고 `run my code` 를 누르면  
캐릭터에 날개가 달리고, 집(?)에서 WINTER LAND로 날아가는 연출..

**코딩 교육적 요소** 함수 호출 (no params)  
goTrip() 같은 느낌으로..

### Scene 3

극지방 같은 배경에 내가 그린 동물들이 일정한 간격을 두고 서 있고,  
내 캐릭터가 날아가면서 동물들에게 인사(?)할 수 있다.

(내 캐릭터)  (동물1)  (동물2)  (동물3)  (동물4)

이렇게 서 있고, 매개변수로 넘겨줄 Int값 만큼 날아가는 것 ~!  
큰 Int가 넘어올 경우를 대비해 `Int값 % 동물 수` (나머지) 에 해당하는 동물을 만난다.  
그렇다고 동물이 4마리인데 7을 넣었다고 3번만 날아가진 않고,  
가능하다면 7번 날아가는데 동물들이 cycle을 돌아서 더 나타나게 구현하고 싶다~!

최대값도 정해놓는게 좋을것 같다.  
예를들어 30번 이상 날게 하면 힘들다고 안 난다고 한다던지 ㅋㅋㅋ

날아가면서 동물들을 지나치고 다 볼 수 있다.

또한, 동물들을 클릭하면 설명이 적힌 카드가 위에 겹쳐져 뜨도록!

**코딩 교육적 요소** Int형 매개변수를 넘겨주는 함수 호출  
flap(times: 4) 같은 느낌..

### Scene 4

Scene 3에서는 동물들이 밝은, 건강한(?) 상태였다면,  
Scene 4에서는 그 동물들이 지구 온난화로 인해 어떻게 변했는지를 보여준다.

전체적으로 어두운 분위기를 연출!  
작동 방식은 Scene 3과 동일하다.  
다만 코딩 교육적 요소에 있어서는 flap(times: )  를 다르게 구현해보는.. 느낌으로  
for 반복문을 사용할 예정이다!

**코딩 교육적 요소** for 반복문  

 ```
for n in 0...[사용자 입력] {
	flap()
}
 ```

### Scene 5

우리가 실천할 수 있는 것들!을 알려주는 뷰  
위에는 빈 폴라로이드 4장이 붙어있고,  
아래에는 해수면 상승으로 인한 자유의 여신상의 부분 잠김 이라든가,,  
탄저균이나 슈퍼파도 등 지구온난화로 인한 다른 변화들을 보여주고,  
폴라로이드 사진을 하나 찍을 때 마다  
빈 폴라로이드에는 사진이 보여지고 변화들도 사라지는 모습을 보여준다.

**코딩 교육적 요소** Boolean

```
var 자전거타기 = true
var 플러그뽑기 = true
var 텀블러쓰기 = true
var 재활용하기 = true
```

모든 값이 true가 돼야 넘어갈 수 있다.  
false일 경우엔 사진 안 찍힘!

### Scene 6

마지막 뷰. 모든 동물들이 Happy~한 상태로 마무리~~



이젠 진짜 구현에 들어가야 할 시간!