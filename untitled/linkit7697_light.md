# 光敏模組

![](../.gitbook/assets/linkit7697_light_00.jpg)

## 專案說明

使用「LinkIt 7697 NANO Breakout」連接「光敏模組」, 每0.5秒讀取光敏模組數值。  
此**光敏模組**包含於「**Education Kit for Linkit 7697**」內。

## 電路圖

**•**	[**LinkIt 7697**  
](https://www.robotkingdom.com.tw/product/linkit-7697/)**•	LinkIt 7697 NANO Breakout  
•	光敏模組**

**光敏模組**是**類比訊號**輸入， 可以接「A0 ~ A3」的 LinkIt 7697 NANO Breakout訊號端上，「A0 ~ A3」腳位在程式碼中以「14 ~ 17」表示。 本範例連接到「**A0**」，程式碼中為「**14**」。

![](../.gitbook/assets/linkit7697_light_01.png)

## 積木畫布

每0.5秒鐘會讀取光敏模組一次， 並顯示在序列埠監控視窗上。

![](../.gitbook/assets/linkit7697_light_02.png)

![](../.gitbook/assets/linkit7697_light_03.png)

產生出的 Arduino 程式如下：

```text
void setup()
{

  Serial.begin(9600);

}


void loop()
{
  Serial.println(analogRead(14));
  delay(500);
}

```

