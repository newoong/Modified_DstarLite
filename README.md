# Modified_DstarLite
This code is for Customized DstarLite Algorithm.

Used this Algorithm in
#### JCDE - A study on unmanned combat vehicle path planning for collision avoidance with enemy forces in dynamic situations
https://academic.oup.com/jcde/article/10/6/2251/7395013

----------

You can run this code through pygame.

- Modified
  1. Moving obstacle

      original DstarLite : Only can add obstacle

      customized DstarLite : Each obstacles can move around.


  2. New Cost

      original DstarLite : Only use k1,k2 value

      customized DstarLite : There are topology costs & obstacle around costs
 
     
<img width="703" alt="스크린샷 2023-06-03 오후 9 34 08" src="https://github.com/newoong/Modified_DstarLite/assets/94604584/71d9fbfa-83fb-439b-9e2e-ecc5f19312c6">

RED : moving obstacle

GRAY : fixed obstacle

BLUE : goal

GREEN : start

APRICOT : topography cost + obstacle around cost (color darkness proportional with cost)

ARROW : current state


%parameters%
  
-graph size : Grid 크기

-obstacle_ratio : Grid 크기에서 모든 장애물 비율

-fixed_obs_ratio : 모든 장애물에서 고정 장애물 비율

-move_chance : 가변 장애물의 매번 움직일 확률

-alpha : calculate_key에서 k1,k2에 더해주는 가변 장애물 주변 cost의 가중치

-beta : calculate_key에서 k1,k2에 더해주는 지형지물의 가중치

-step : 나의 위치가 가변 장애물의 몇칸안에 들어왔을 때 Rescan할지

-influence : 가변 장애물 cost의 영역 크기

-smart : 가변 장애물이 나의 위치를 기반하에 움직일지 랜덤하게 움직일지

-detectability : smart=True일 때, 나의 위치 감지력
