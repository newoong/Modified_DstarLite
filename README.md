# Modified_DstarLite
This code is for Customized DstarLite Algorithm.

You can run this code throgh pygame.

- Modified
  1. Moving obstacle

      original DstarLite : Only can add obstacle

      customized DstarLite : Each obstacles can move around.


  2. New Cost

      original DstarLite : Only use k1,k2 value

      customized DstarLite : There are topology costs & obstacle around costs
 
     
<img width="703" alt="스크린샷 2023-06-03 오후 9 34 08" src="https://github.com/newoong/Modified_DstarLite/assets/94604584/71d9fbfa-83fb-439b-9e2e-ecc5f19312c6">

RED : obstacle

BLUE : goal

GREEN : start

APRICOT : topography cost + obstacle around cost (color darkness proportional with cost)

ARROW : current state
