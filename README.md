# jiqimao
通过语音识别模块控制机器猫实现前进后退摇头摆尾等功能

  /* Time base configuration */		 
	/* PWM信号电平跳变值 */
//((1+TIM_Prescaler )/72M)*(1+TIM_Period )=((1+71)/72M)*(1+19999)=20000us	
//u16 CCR4_Val =499;500us,0度 
//u16 CCR4_Val =999;1000us,45度 
//u16 CCR4_Val =1499;1500us,90度
//u16 CCR4_Val =1999;2000us,135度 
//u16 CCR4_Val =2499;2500us,180度 

舵机信号线引脚号

1号舵机       B6       已测       左前
2号舵机       B7       已测       右前
3号舵机       B8       已测       左后
4号舵机       B9       已测       右后
5号舵机       A0       已测       头
6号舵机       A1       已测       尾
7号舵机       A2       已测       
8号舵机       A3       已测  



		//其他舵机控制可别对应TIM_SetCompare(1,2,3,4),角度参数不变
		//舵机分别为舵机1号（控制齿条上下）舵机2（控制套筒开合）舵机3（控制钩子竖直运动）舵机4（控制钩子水平运动），对应TIM_SetCompare(1,2,3,4)。
  /* Time base configuration */		 
	/* PWM信号电平跳变值 */
//((1+TIM_Prescaler )/72M)*(1+TIM_Period )=((1+71)/72M)*(1+19999)=20000us	
//u16 CCR4_Val =499;500us,0度 
//u16 CCR4_Val =999;1000us,45度 
//u16 CCR4_Val =1499;1500us,90度
//u16 CCR4_Val =1999;2000us,135度 
//u16 CCR4_Val =2499;2500us,180度 
//		/* 最中间的位置 */		
//		TIM_SetCompare4(GENERAL_TIM5,1499);
//		delay_ms(2000);
//		/* 向后90度 */  
//		TIM_SetCompare4(GENERAL_TIM5,2499);
//		delay_ms(2000);
//		/* 最中间的位置 */		
//		TIM_SetCompare4(GENERAL_TIM5,1499);
//		delay_ms(2000);
//		/* 向前90度 */
//		TIM_SetCompare4(GENERAL_TIM5,499);
//		delay_ms(2000);
//		break;
