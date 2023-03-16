# quantize model

* [https://ithelp.ithome.com.tw/articles/10267328](https://ithelp.ithome.com.tw/articles/10267328)
* quantization
* continuous range to finite range of discreet values
* 2.568 -> 1,2,3
* time analogy
* 24 bits / 8 bits / 1 bit per pixel
* 不同於 normalization
  * 自己的誤解 : normalization (scale 完後仍是 continous)
  * quantization 不是, 為 discreet (離散)
* quantization
  * unsinged int 8 bit max = 255
  * image 0\~255 / 255.0 = 0\~1
  * dynamic range?
    * 範圍大: 解析度差 (0, 0.49 都變成 0)
    * 8 bit quantize \* scale = floating range
    * ex: floating range 100 \* 255.0
    * scale > 0.5 大
    * scale < 0.01 以下, 還不錯準的 model
    * scale 可用於表達 dynamic range, 藉此判斷 quantization 效果好不好
  * offset = - zero point (通常我們會去 - offset)
    * offset
    * zero point
    * 可以用 y = ax + b 去想, a: scale, b: offset
    * x\_quant = (x\_ori - offset) \* scale
  * bit-width b, 例如 8 bit = 255 = 2 ^8 - 1
  * symmetric quantization (對稱)
    * 注意重點在公式 x\_ori = x\_quant \* scale
  * asymmetric quantization (非對稱)
    * 公式 x\_ori = (x\_quant - zero point)\* scale
    * x\_ori\_min = - sacle \* zeropoint (= quant的0)
    * zeropint = quant 後固定位置 = s(x\_ori\_0 - zero point),  x\_ori\_0 = zero point
    * 優點 0 可以被固定, 更精準
    * [https://arxiv.org/pdf/2106.08295.pdf](https://arxiv.org/pdf/2106.08295.pdf)
    * [https://zhuanlan.zhihu.com/p/555320173](https://zhuanlan.zhihu.com/p/555320173)
    * [https://pic3.zhimg.com/80/v2-bd405292a0ef06f1f8257e80663d5eda\_1440w.webp](https://pic3.zhimg.com/80/v2-bd405292a0ef06f1f8257e80663d5eda\_1440w.webp)
* post training quantization

