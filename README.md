# 러브레이스 동적 날씨 카드 (feat. Naver weather)

Originally created for the [old UI](https://community.home-assistant.io/t/custom-ui-weather-state-card-with-a-question/23008) converted by @arsaboo and @ciotlosm to [Lovelace](https://community.home-assistant.io/t/custom-ui-weather-state-card-with-a-question/23008/291) and converted by @bramkragten. 

This card uses the awesome [animated SVG weather icons by amCharts](https://www.amcharts.com/free-animated-svg-weather-icons/).

![image](https://github.com/plplaaa2/HA-weather-card-custom/assets/124797654/ba486511-69c9-4576-8465-4f42550ed77b)

Thanks for all picking this card up.

## 설치법:

**Special Thanks**

HACS 네이버 날씨 제작자 miumida님
<br>

**변경사항**

| Version | Date        | 내용              |
| :-----: | :---------: | --------------------------------------------------------------------------------------- |
| v1.0  | 2024.04.25  | First version  |
| v1.1  | 2024.05.02  | 체감온도 현재온도 차이에 따른 색상 변화 안되는 문제 해결  |

# 주의사항

기본 센서 값이 'sensor.naver~' 로 시작되는 것만 사용 가능하기 때문에<br> 
한글을 영문으로 쓴 센서값 'sensor.gangsuryang' 일 경우<br> 
기기 및 서비스 -> 네이버 날씨 -> 구성요소에 들어가 센서 값을 'sensor.naver~' 로 다시 수정하여야 사용 가능

# 설치방법

1. [네이버 날씨](https://github.com/miumida/naver_weather)설치
2. Weather-card 설치 ( HACS -> frontend -> : -> custom repositories)
```yaml
   repositories
   https://github.com/plplaaa2/weather-card
   category
   lovelace
```
3. 


# 쉬운 적용방법

1. 대쉬보드 -> 편집 -> 리소스 관리
2. 예) /hacsfiles/weather-card/weather-card.js?hacstag=192732636150 선택
3. hacstag=192732636150 <- 숫자 하나 더 추가
<br>※ 브라우저 캐시 삭제 안해도 됩니다.
