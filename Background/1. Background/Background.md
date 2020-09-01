# background! 
이름에서 보이지만 background와 관련된 속성이 있다. 

## background-color
배경에 색상을 넣고 싶을 때 사용하는 속성이다.

hex, rgb, rgba 를 사용해서 색상을 지정하면 된다. 
만약 hex, rgb, rgba가 뭔지 모르겠다면 Typography를 다시 한번 보자!

## background-image 
배경에 이미지를 넣을 때 사용한다.

url()을 같이 사용해서 기능을 수행 하는데, 이것은 내가 사용할 이미지가 있는 경로를 url()이라는 함수 안에 넣어줘야 한다.

## background-repeat
기본적으로 배경에 image를 넣으면 반복해서 들어간다. 

하지만 반복을 원하지 않는 경우 해당 속성을 사용해서 

```
background-repeat : no-repeat;
```
을 사용하면 반복되지 않는다.

## background-size
배경에 있는 이미지의 size를 설정할 때 사용한다.

contain, cover, custom 3가지 속성을 사용할 수 있다.

contain 은 내가 넣으려는 이미지가 배경보다 작은경우, 배경에 이미지가 모두 표시 될 수 있도록 이미지를 줄인다.

cover 는 요소에 빈 공간을 남기지 않고 꽉 채워준다.

custom 은 임의의 값을 넣어주면 된다.

```
background-size : 100% auto  // <- 가로는 100% 세로는 자동으로
```

## background-position
배경 이미지를 어떻게 위치 시킬지 설정한다.

x, y 2개를 설정해야 한다.

```
background-position : center center // <- x = center, y = center 
```

이때 x y를 center 이렇게 설정하지 말고 10px, 50px 이런식으로 사용할 수 있다.

하지만 가장 많이 사용하는 방식이 x,y 모두 center 로 지정하는 방식이다.