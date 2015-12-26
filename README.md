# 实例YGBanner代码

# UIScrollView复用，自动循环滚动，以及点击事件

NSArray *imageNames = @[@"1.jpg", @"2.jpg", @"3.jpg", @"4.jpg"];

YGBanner *banner = [[YGBanner alloc] initWithFrame:CGRectMake(0, 0, self.view.bounds.size.width, 160) imageNames:imageNames imageHandle:^(NSInteger index) {

    NSLog(@"点击了YGBanner第%ld张图", index);
}];

[self.view addSubview:banner];
