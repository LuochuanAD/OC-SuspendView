# OC-SuspendView
悬浮视图:按钮/图片/轮播图/gif图/音频/视频/自定义view




悬浮按钮:
![image](https://github.com/LuochuanAD/OC-SuspendView/blob/master/SuspendView/suspendButton.gif)

悬浮图片:
![image](https://github.com/LuochuanAD/OC-SuspendView/blob/master/SuspendView/suspendImageView.gif)

悬浮Gif图
![image](https://github.com/LuochuanAD/OC-SuspendView/blob/master/SuspendView/suspendWebView.gif)

悬浮滚动图
![image](https://github.com/LuochuanAD/OC-SuspendView/blob/master/SuspendView/suspendScrollView.gif)

悬浮视频
![image](https://github.com/LuochuanAD/OC-SuspendView/blob/master/SuspendView/suspendVideo.gif)



使用:


/**悬浮视图的类型

 BUTTON    =0,//按钮
 
 
 IMAGEVIEW =1,//图片
 
 
 GIF       =2,//gif图
 
 
 MUSIC     =3,//音乐界面
 
 
 VIDEO     =4,//视频界面
 
 
 SCROLLVIEW =5,//滚动多图
 
 
 OTHERVIEW =6//自定义view
 
 
 */
 
 
 
- (void)viewDidLoad {


    [super viewDidLoad];
    
    
    
    LCSuspendCustomBaseViewController *suspendVC=[[LCSuspendCustomBaseViewController alloc]init];
    
    
    
    suspendVC.suspendType=SCROLLVIEW;
    
    
    
    [self addChildViewController:suspendVC];
    
    
    
    [self.view addSubview:suspendVC.view];
    
    
    
}
