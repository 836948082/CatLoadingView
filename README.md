# Android CatLoadingView

This project idea is from [Link](http://mp.weixin.qq.com/s?__biz=MjM5MDMxOTE5NA==&mid=402703079&idx=2&sn=2fcc6746a866dcc003c68ead9b68e595&scene=2&srcid=0302A7p723KK8E5gSzLKb2ZL&from=timeline&isappinstalled=0#wechat_redirect) .<br>
Thanks for the idea.<br>

I like the animation in that picture.<br>

![](https://github.com/836948082/CatLoadingView/blob/master/image/image.gif)

..as you see right now,wish you like it.

### Step

Import this project into android studio..it's build with it.

###  Usage

#### Gradle

```
compile 'com.android.support:design:23.2.1'
```

####  config in java code

    CatLoadingView mView;


    @Override protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        
        mView = new CatLoadingView();
        findViewById(R.id.button).setOnClickListener(
                new View.OnClickListener() {
                    @Override public void onClick(View v) {
                        mView.show(getSupportFragmentManager(), "");
                    }
                });
    }

## TODO

This view is adjust in Nexue5 but not test in the other size screen .