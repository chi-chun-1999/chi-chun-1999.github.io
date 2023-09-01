---
title: "CVAT Segmentation Polygon Shape Mode"
date: 2023-08-29T18:46:34+08:00
draft: True
tags: ['cvat']
categories: ['cvat']
---

# 使用方式
- 請在側邊欄選擇 `polygon` 來進行標記，並選擇要進行標記的 __Label__，點擊 __Shape__。


	{{< img src="/posts/cvat/images/Pasted%20image%2020230827115906.png" size="medium" title="">}}


- 在進行標記時，可以用以下兩種方式增加新的點，並附上兩種方式的所呈現的效果：
	1. 滑鼠點擊
	2. 滑鼠移動並按住`shift` 鍵

	<!--{{<img src="/posts/cvat/images/" size="self" width="">}}-->



	|{{<img src="/posts/cvat/images/螢幕錄製%202023-08-25%20下午7.52.23.gif" size="self" width="70%">}} |{{<img src="/posts/cvat/images/螢幕錄製%202023-08-27%20下午1.10.18.gif" size="self" width="70%">}} |
	|:-----:|:-----:|
	|  滑鼠點擊  |  滑鼠移動 + 按住`shift` 鍵  |

- 最後標記結束，可以選擇按左上角的 `Done`或是按下 `n`鍵即完成標記，標記框的顏色會從灰色轉成 label 對應的顏色。
	{{<img src="/posts/cvat/images/Pasted%20image%2020230827143619.png" size="self" width="40%">}}
	{{<img src="/posts/cvat/images/螢幕錄製%202023-08-27%20下午1.10.18%201.gif" size="self" width="50%">}}



# 其他操作事項

- 在進行標記的同時，如果發現標記錯誤，我們可以按下 __滑鼠右鍵__ 即可取消前一個標記的點。
{{<img src="/posts/cvat/images/螢幕錄製%202023-08-27%20下午2.25.36.gif" size="self" width="" >}}
- 在標記時按下`ESC`會取消所有標記的灰色點。
{{<img src="/posts/cvat/images/螢幕錄製%202023-08-27%20下午2.44.09.gif" size="self" width="">}}
-  __標記完成後__ 發現需要增加新的點，可以按下`shift`鍵並點擊要增加的地方。
{{<img src="/posts/cvat/images/編輯標記點.gif" size="self" width="">}}
- __標記完成後__ 發現需要刪除標記點，可以點擊滑鼠右鍵選擇 `delete point`或是滑鼠點擊加上 `alt` 鍵。
{{<img src="/posts/cvat/images/delete_point.gif" size="self" width="">}}


# 參考資料

[Manual drawing | CVAT (opencv.github.io)](https://opencv.github.io/cvat/docs/manual/advanced/annotation-with-polygons/manual-drawing/)

