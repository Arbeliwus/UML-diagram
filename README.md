# UML-diagram
## 什麼是類別？什麼是對象？他們的關係是什麼？
類別：類別是具有相同屬性和服務的一組物件的集合。為屬於該類別的所有物件提供了統一的抽象描述，其內部包括屬性和服務（方法）兩個主要部分。

對象：對像是系統中用來描述客觀事物的實體，是構成系統的一個基本單位。一個物件由一組屬性和這組屬性進行操作的一組服務組成。從更抽象的角度來講，物件是問題域或實現域中某些事物的一個抽象，她反應該事物在系統中需要保存的資訊和發揮的作用；它是一組屬性和有權對這些屬性進行操作的一組服務的封裝體。客觀世界是由物件和物件之間的連結所組成的。

類別與對象的關係如磨俱與鑄件的關係，類別的實例化結果就是對象，而對一類對象的抽象就是類別。類別描述了一組具有相同特徵（屬性）和形同行為（方法）的對象

## 什麼是類別圖？
類別圖一反應類別的結構（屬性、操作）以及類別之間的關係為主要目的，描述了軟體系統的結構，是一中靜態建模方法。

類別圖中的「類別」與物件導向語言中的「類別」的概念是對應的，是現實世界中事物的抽象。

![](https://img-blog.csdnimg.cn/20181202110640986.png)

用例圖後面為什麼是畫類別圖，而不是其他圖，類別圖產生於什麼階段，由誰來繪製，類別圖它的作用是什麼？因為依照軟體工程的生命週期來運作的話，需求分析階段後便是設計階段了，而類別圖產生於設計階段，由系統設計師繪製，其作用是描述系統的架構結構、指導程式設計師編碼。它包括系統中所有有必要指明的實體類、控制類、界面類及與特定平台有關的所有技術性資訊。

### UML類別圖如何繪製？

1) 類的組成
從上到下分為三部分，分別是類別名稱、屬性、操作。
![](https://img-blog.csdnimg.cn/20181202113652178.png)

2) 接口
一組操作的集合，只有操作的聲明而沒有實現。介面圖與類別圖的主要差異在於頂端的<<interface>>顯示。第一行是介面名稱，第二行是介面方法。介面還有另一種表示方法，俗稱棒棒糖表示方法。唐老鴨是能講人話的唐老鴨，實現了講人話的介面。如圖：
![](https://img-blog.csdnimg.cn/20181202114053368.png)

3) 抽象類
不能被實例化的類，一般至少包含一個抽像操作，與類別圖的主要差異在於抽象類別的名稱、方法為斜體。
![](https://img-blog.csdnimg.cn/20181202114551212.png)

4) 模板類
一種參數化的類，在編譯時把模板參數綁定到不同的資料型別，產生不同的類。

![](https://img-blog.csdnimg.cn/20181202114723341.png)
 ### 類的關係

1) 關聯關係
描述了類別的結構之間的關係，具有方向、名字、角色和多重性等資訊。

![](https://img-blog.csdnimg.cn/2018120212300185.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L0Vsc2ExNQ==,size_16,color_FFFFFF,t_70)

一般的關聯關係語意較弱，也有兩種語意較強，分別是聚合和組合

3) 泛化關係
在物件導向中一般稱為繼承關係，存在於父類別與子類別、父介面與子介面
![](https://img-blog.csdnimg.cn/20181202123747195.png)

![](https://img-blog.csdnimg.cn/2018120212383192.png)

3) 實現關係
對應於類別和介面之間的關係

![](https://img-blog.csdnimg.cn/20181202123938258.png)

5) 依賴關係UML類別圖依賴關係是一種使用關係，特定事物的改變有可能會影響到使用該事物的事物，反之不成立。在你想要顯示一個事物使用另一個事物時使用，兩個元素之間的一種關係，其中一個元素（服務者）的變化將影響另一個元素（客戶），或向它（客戶）提供所需資訊.

### 類圖心智圖
![](https://img-blog.csdnimg.cn/20181202213337549.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L0Vsc2ExNQ==,size_16,color_FFFFFF,t_70)
### 繪製類圖
![](https://img-blog.csdnimg.cn/20181202212904310.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L0Vsc2ExNQ==,size_16,color_FFFFFF,t_70)
### 對象圖
1) 什麼是對象圖
物件圖也是靜態圖的一種，但是物件圖描述一個系統在某個時刻的靜態結構，顯示的是物件與物件之間的關係，而類別圖描述所有可能的情況。

2) 繪製對象圖
![](https://img-blog.csdnimg.cn/20181205200304898.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L0Vsc2ExNQ==,size_16,color_FFFFFF,t_70)


### 參考網站:https://blog.csdn.net/Elsa15/article/details/84700651

