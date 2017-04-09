# 居中一张图片
>在不被后台支持图片剪裁的情况下，用于用户上传信息中的图片需要按照一个居中规则来展示，从而统一样式

## 示例
![示例图片](http://img.ojutao.com/14913124889930e58e160-bba5-4d24-84bc-836e7da2c710bGw7DncADK.png)

### 如何使用
* 直接使用：引入centerImg.js 文件 通过centerImg(dom)
* ES6：在centerImg.js最后加入 ``` export centerImg; ```,在使用页面引``` import centerImg from 'centerImg.js'

#### code
``` HTML
  <ul>
    <li>
      <a class="item-link">
        <img src="xxx.png" alt="xxx"/>
      </a>
    </li>
  <ul> 
  <script src="src/centerImg.js"></script>
  <script>
      [].forEach.call(document.querySelectorAll('.item-link'),function(imgFa){
        centerImg(imgFa);//第二个参数为number 为过度效果持续的时间
      });
  </script>
```