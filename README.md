# ShowcaseCoordinator

ShowCaseCoordinator will inflate layout,and move the needMoveView which contain the indicatorView,
let the indicatorView right above the targetView.

自动定位的引导页，可以将引导页上的某个View对齐到指定的TargetView上。具体使用可以看Demo


## Effect picture

my_show_case_layout.xml

<img src="https://github.com/lylwo317/MyShowcaseLayout/blob/master/screenshot/layout-2016-08-17-132455.png" width="400">

MainActivity

<img src="https://github.com/lylwo317/MyShowcaseLayout/blob/master/screenshot/layout-2016-08-17-132712.png" width="400">

Use ShowCaseCoordinator in MainActivity

<img src="https://github.com/lylwo317/MyShowcaseLayout/blob/master/screenshot/device-2016-08-17-134533.png" width="400">




## Usage


``` java
 new ShowcaseCoordinator.Builder(this, R.layout.my_show_case_layout)
                .addShowcase(tvHelloFirst, R.id.imageView_first, R.id.llyt_move_first)
                .addShowcase(tvHelloSecond, R.id.imageView_second, R.id.llyt_move_second)
                .addShowcase(tvHelloThird, R.id.imageView_third, R.id.llyt_move_third)
                .build();
```

