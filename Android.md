## Android  
### 2018年5月11号  
记录自己Android学习之路  
**控件**  
visibility控件属性，控制控件是否可见，其属性值有三个："visible","invisible","gone".而INVISIBLE和GONE的主要区别是：当控件visibility属性为INVISIBLE时，界面保留了view控件所占有的空间；而控件属性为GONE时，界面则不保留view控件所占有的空间.  
>**可见（visible)**    
>XML文件：android:visibility="visible"  
>Java代码：view.setVisibility(View.VISIBLE);  
>**不可见（invisible)**  
>XML文件：android:visibility="invisible"  
>Java代码：view.setVisibility(View.INVISIBLE);  
>**隐藏（GONE)**  
>XML文件：android:visibility="gone"  
>Java代码：view.setVisibility(View.GONE);    
  
### 2018年5月16号  
```
webView.getSettings().setJavaScriptEnabled(true);//设置内嵌浏览器支持Javascript脚本语言
webView.setWebViewClient(new WebViewClient());当页面跳转时依旧在内嵌浏览器中
webView.loadUrl("http://www.baidu.com");//将网址传入，以百度为例
```
webview控件，在自己的应用程序中嵌入一个浏览器。  
### 2018年5月23号  
ScrollView控件，可以以滚动的形式查看屏幕外的内容。是Framelayout的子类，但是该控件中只能放一个组件，要想放多个组件必须放置一个布局
```
<ScrollView
android:id="@+id/myscollView"  
android:layout_width="match_parent" 
android:layout_height="wrap_content" > 
//这里只能放一个布局或控件
//一般是放LinearLayout布局
</ScrollView>
```
removeAllViews()是ViewGroup中的一个移除所有子view的方法，得到一个空的layout布局。  
在ViewGroup中还有一个移除子view的方法是removeAllViewsInLayout(),该方法会先测量当前的布局, 一旦调用该方法,只能移除已经自身布局中已计算好的所包含的子view.  
方法removeAllViewsInLayout()源码:  
```
/** 
     * Call this method to remove all child views from the 
     * ViewGroup. 
     */  
    public void removeAllViews() {  
        removeAllViewsInLayout();  
        requestLayout();  
        invalidate(true);  
    } 
```
方法removeAllViews()除了调用removeAllViewsInLayout()方法还调用了requestLayout()方法，比removeAllviews()方法移除的更彻底。  
