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
ScrollView控件，可以以滚动的形式查看屏幕外的内容。  
webview控件，在自己的应用程序中嵌入一个浏览器。  
