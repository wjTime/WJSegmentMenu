# WJSegmentMenu
a simple segment menu 分段选择菜单

1.创建
    WJSegmentMenu *segmentMenu = [[WJSegmentMenu alloc]initWithFrame:CGRectMake(0, 64, self.view.frame.size.width, 40)];
    segmentMenu.delegate = self;
    [segmentMenu segmentWithTitles:@[@"完成",@"未完成",@"待接单"]];
    [self.view addSubview:segmentMenu];
    
2.代理方法
    - (void)segmentWithIndex:(NSInteger)index title:(NSString *)title;
