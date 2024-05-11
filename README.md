# Lovelace Weather Card Custom (feat. Naver weather)

Originally created for the [old UI](https://community.home-assistant.io/t/custom-ui-weather-state-card-with-a-question/23008) converted by @arsaboo and @ciotlosm to [Lovelace](https://community.home-assistant.io/t/custom-ui-weather-state-card-with-a-question/23008/291) and converted by @bramkragten. 

This card uses the awesome [animated SVG weather icons by amCharts](https://www.amcharts.com/free-animated-svg-weather-icons/).

Thanks for all picking this card up.

# 적용 예

![image](https://github.com/plplaaa2/HA-weather-card-custom/assets/124797654/17ff189d-5a7e-4c97-8838-1cdc1886e2ac)

 평소

![image](https://github.com/plplaaa2/HA-weather-card-custom/assets/124797654/62c5b8c0-efb1-46ce-98d1-e4aba81b76a4)

비가 오려고 할 때

![image](https://github.com/plplaaa2/HA-weather-card-custom/assets/124797654/ba486511-69c9-4576-8465-4f42550ed77b)

비 올때

**변경사항**

| Version | Date        | 내용              |
| :-----: | :---------: | --------------------------------------------------------------------------------------- |
| v1.0  | 2024.04.25  | First version  |
| v1.1  | 2024.05.02  | 체감온도 현재온도 차이에 따른 색상 변화 안되는 문제 해결  |


# 설치법

## 주의사항

기본 센서 값이 'sensor.naver~' 로 시작되는 것만 사용 가능하기 때문에

예를 들어 한글을 영문으로 쓴 센서값 'sensor.gangsuryang' 일 경우 기기 및 서비스 -> 네이버 날씨 -> 구성요소에 있는 

모든 센서 값을 'sensor.naver~' 로 다시 수정하여야 사용 가능

![image](https://github.com/plplaaa2/HA-weather-card-custom/assets/124797654/bf9cdd58-a41e-439f-b35d-f1776ff557c1)

## 설치방법

1. [네이버 날씨](https://github.com/miumida/naver_weather)설치
   
   **Special Thanks** HACS 네이버 날씨 제작자 miumida님
   
4. 기존 weather-card 삭제(중복이라)
5. Weather-card 설치 ( HACS -> frontend -> : -> custom repositories)
```yaml
   repositories : https://github.com/plplaaa2/weather-card
   category : lovelace
```
4. repositories 목록에서 plplaaa2/weather-card 클릭
5. '다운로드' 클릭
6. 대쉬 보드 편집 -> 카드 추가 -> weather로 검색 후 사용자 weather-card 추가
