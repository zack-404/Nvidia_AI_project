# Nvidia AI 實作

## 動機

因為這學期的多元選修，我上了```AI人工智慧與科學探究```。在這堂課裡，老師有講到關於AI人工智慧的應用，同時也跟我們說有這個課程。可以上，因為我想在更深入的了解有關AI人工智慧的實作，於是就參加了這個課程。

## 課程大綱

1.  深度學習簡介 
2.  神經網路訓練方式 
3.  捲基神蹟網路
4.  資料加強與部屬
5.  預先訓練模型
6.  先進架構


## 重點紀錄

1. 早期是因為資料與運算能力不足，已導致人工智慧的發展遇到了瓶頸
2. 運用一些數學函數作為激活函數或是矩陣的運算，例如：Sigmoid、ReLU、或是常見線性函數、抑或是矩陣相加
3. 若若是將圖片化為縣性資料，那便有可能損失許多資訊，因此矩陣變成了比函數好的解法，那變成了卷基神經網路
4. 可以運用一些縮放、選轉等技巧將目標物放大，或是可以用矩陣的乘法，改變圖的亮度等等之類的
5. 可以使用一些已經設計好的模型以URL的方式插入Python，再加上一些遷移學習，便可產收我們想要的模型
6. 遞歸神經網路，大意就是讓目標多跑幾次網路，以提升準確率；GAN生成對抗網路，這個模醒會產生＂產生器＂與＂與＂鑑別氣＂讓目標跑兩個模型並對忼產生結果。

## 心得

上完這個實作課最大的收穫就是----AI是個十分複雜的領域，也十分仰賴數學基礎。

在AI的領域裡，一樣可以跟許多CS領域一樣可以分成理論(演算法)與應用(實作)，雖然這次是比較偏重於實作的，但老師也有帶到一些演算法的內容。光是那一點的演算法，就已經讓我聽不懂了，不過這正是學習新知有趣的地方，把原本都不懂的東西，懂了點皮毛，或甚至是成為專家，也許之後也可以朝這方面發展。

演算法的部分，就似乎是用那些感覺很簡單的數學函數，去做合成函數，或或者是找個矩陣家家家，然後神奇的事情就發生了，模型就產生了。

其實在上課的時間，我幾乎都是處於一個聽不懂的狀態，只是好像略懂了那些演算法模型，就有種 用這個Module裡的一些函示，跑一下，模型就做出來了 ，過程中就是整個"蛤"，感覺都是在變魔術。不過後來自己再去複習或是去查單字的時候，就比較懂了，哪些函式是做甚麼的，即使忘了，還是可以從字面上大概推出是在做甚麼的。
例如：

    assessment      評估
	horizontal      水平
	vertical        垂直
	batch           批處理
	ampere          安培
	epochs          紀元
	fraction        分數
	derive          派生
	propagate       傳播
	perceptron      感知器
	context         語境
	transpose       轉置
	hierarchical    分層
	gradient        梯度



也經過這次的課程，多了台有Nvidia GPU的Server可以使用，也許未來可以多多善用這個資源。

## 成果
[測驗成果](https://github.com/zack-404/Nvidia_DLI_project/blob/main/07.py)

```
評估模型
在理想狀況下，現在你的模型驗證準確度應該會達到 92% 或以上。
如果不是如此，建議你回到先前步驟執行更多 Epoch 的訓練，或是調整資料增強。

達到理想的驗證準確度後，請執行下列儲存格來評估模型。
評估函數會回傳一個元組(Tuple)，其中第一個值表示損失，第二個值表示準確度。
若要通過本測驗，模型的準確度值必須為 92% or higher。

model.evaluate(valid_it, steps=valid_it.samples/valid_it.batch_size)
11/10 [================================] - 4s 346ms/step - loss: 1.0733 - categorical_accuracy: 0.9757
[1.073278784751892, 0.975683867931366]
執行測驗
若要測驗模型，請執行以下兩個儲存格。

注意： run_assessment 會假定你的模型名稱為 model，以及你的驗證資料迭代器名稱為 valid_it。
若你修改了這些變數名稱，請更新傳遞至 run_assessment的引數名稱。

from run_assessment import run_assessment
run_assessment(model, valid_it)
Evaluating model 5 times to obtain average accuracy...

11/10 [================================] - 4s 349ms/step - loss: 1.0734 - categorical_accuracy: 0.9726
11/10 [================================] - 4s 381ms/step - loss: 1.0750 - categorical_accuracy: 0.9696
11/10 [================================] - 4s 342ms/step - loss: 1.0714 - categorical_accuracy: 0.9787
11/10 [================================] - 4s 347ms/step - loss: 1.0794 - categorical_accuracy: 0.9666
11/10 [================================] - 4s 347ms/step - loss: 1.0695 - categorical_accuracy: 0.9818

Accuracy required to pass the assessment is 0.92 or greater.
Your average accuracy is 0.9739.

Congratulations! You passed the assessment!
See instructions below to generate a certificate.
```

## 證書
![](https://i.imgur.com/8eXQrL0.png)

## Markdown檔案

> HackMD	https://hackmd.io/@zack-404/Nvidia_DLI

## 課程檔案(含程式碼)

> Github	https://github.com/zack-404/Nvidia_AI_project
