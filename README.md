# ball
碰碰球  
碰撞： 
![image](https://github.com/jjjinnni/ball/blob/main/ball.png)  
小球与window和小板块碰撞的动画；  
（1）在画布上显示球的运动，则在绘制小球时，一般围绕圆的中心点确定球的x、y；圆的中心点表示小球的实际位置。因此，圆的半径r很重要，需要在（x,y）上进行加减处理，才能知道此刻的小球有没有撞到window上；实际上不是计算（x,y），而是加减半径r后，再判断小球实际撞到的是哪个部分。  
（2）为了表现出小球的运动，添加VX和VY的运动向量；因此，根据VX和VY的大小，小球就能运动；如，当小球运动到window的左侧边框时，即小球切在边框，（x-r）的值会变成0，故能判断出撞到window的左侧；小球碰撞后，VX和VY的值也会发生变化，此时对vx*（-1），x值变小，y值会增加，故小球的方向从向左变成向右；同理，当小球运动到window的上面，y值就会变小，x值会增加，故小球向右下角运动。  
source: https://www.youtube.com/watch?v=sLCiI6d5vTM
