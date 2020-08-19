# Typography?? 

typography는 사용자에게 읽기 좋은 텍스트를 제공하기 위해 텍스트를 디자인한다.

## 배울 속성

### 1. font-size : 글자의 크기를 지정한다.
사용할 수 있는 단위는 3가지가 있는데, px, em, rem이 있다. 

px은 절대 단위로 어디서든 고정된 값을 가진다.
em, rem은 상대적으로 비례한 값을 가진다. 
=> em은 실제로 적용된 font size를 말한다. 
=> rem은 root(html 태그)의 font size를 말한다.

일반적으로  em과 rem보단 px을 사용한다.

### 2. line-height : 줄 간격을 지정한다.
마찬가지로 px, em, rem으로 단위를 사용할 수 있다.

일반적으로 em을 사용한다.
=> 현재 태그에 적용된 font size에서 얼마나 띄울 것인가?! 라는 이유로 그렇다!
=> 이렇게 line-height를 em으로 사용할 때
<code>line-height : 1.5</code> 이렇게 단위를 빼고 적는 것이 관례이다. 

그 외 px과 rem은 단위를 적어야 한다.

※ 한가지 팁으로 line-height를 사용하면 줄의 가장 가운데에 배치가 된다.
그러므로 수직으로 정렬할 때 사용할 때가 있다.

### 3. letter-space : 글자 간 간격을 지정한다.
px과 em을 단위로 사용한다.

line-height와 마찬가지로 em을 기본적으로 사용한다.
=> 하지만 em을 생략할 순 없다.

### 4. font-family : 폰트를 설정할 때 사용한다.
```
.text {
    font-family : 'Poppins';   <- Poppins라는 font를 적용해라 
    font-family : 'Poppins', sans-serif; <- Poppins라는 font를 적용해라 만약에 없다면 sans-serif 필체중 아무꺼나 적용해라
    font-family : 'Poppins', 'Roboto', sans-serif; <- Poppins라는 font를 적용해라 만약 없다면 Roboto를 적용해라 그것도 없다면 sans-serif 중 아무꺼나 적용해라
}
```
위와 같이 사용한다.

여기서 sans-serif라는 것을 처음보는데,
serif는 글자에 삐침?(명조체??) 이 있는것을 말하며 sans-serif는 굵기가 일정한(고딕?) 것을 말한다.

위 코드에서 Poppins와 Roboto는 serif보단 sans-serif에 가깝기 때문에 sans-serif를 붙이고 serif에 가깝다면 serif를 붙인다.

### 5. font-weight : 폰트의 굵기를 나타낸다.
100  Thin
     Thin Italic
300  Light
     Light Italic
400  Regular
     Regular Italic
500  Medium
     Medium Italic
700  Bold
     Bold Italic
900  Black

위와 같이 굵기가 있는데 100단위로 증가한다.
여기서 가장 많이 사용하는 것이 400 Regular와 700 Bold이다.

### 6. color : 글자의 색상을 나타낸다.
이때 사용하는 방식이 3가지가 있다.

hex, rgb, rgba 이렇게! 

#0066ff 와 같이 색상을 문자로 나타내는 방식을 hex 방식이라고 한다.
rgb(0,102,255) 와 같이 rgb로도 나타내고
rgba(0,102,255,1)로 rgba로도 나타낸다. 마지막 1은 투명도로 0.5일 경우 50%의 투명도를 나타낸다. 