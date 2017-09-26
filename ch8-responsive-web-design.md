# 响应式web设计

+ 响应式web设计的历史和原因
+ 视口（viewport）、媒体类型（media types）、媒体查询（media queries）的原理
+ 创建响应式网站时的“移动优先”策略
+ 何时何地创建断点
+ 使用flexbox、grid、multi-column响应式布局的例子
+ 响应式排版和响应式媒体内容

## 响应式例子

### 简单例子开始

对于移动设备等很窄的视口而言，通常情况下简单布局足够了。
 
 ### 创建第一个媒体查询
 
 ```css
 @media only screen and (min-width: 35em){
   .row-quartet > * {
     width: 50%;
   }
   .subcategory-featured {
     width: 100%;
   }
 }
 ```

断点。

### 更多断点

继续增加浏览器窗口的大小，就会有更大的空间 -- 理应得到更高效的利用。大约800px（50em），

```css
@media only screen and (min-width: 50em) {
 .row-quartet > * {
   width: 25%; 
  }
  .subcategory-featured {
    width: 50%;
  }
}
```

```css
@media only screen and (min-width: 70em) {
 .subcategory-header {
   width: 20%;
  }
  .subcategory-content {
    width: 80%;
  }
}
```

## 响应式的起源

Ethan Marcotte. 2010. 《responsive-web-design》

John Allsopp. 2000. 《A Dao of Web Design》

到了2010年，媒体查询得到了更广泛的支持，再加上移动设备更加流行，Ethan将这些技术结合起来，给了一个新的术语：响应式web设计。

### css之外的响应式

JS. hamburger menu.

pattern: 先加载一个核心资源，根据设备再加载更多。响应式设计本质上就是**渐进增强**。

## 浏览器视口（viewport）的原理

css像素不同于物理像素，与物理像素的比例，受到硬件、操作系统、浏览器、用户缩放等因素影响。
设备像素比dpr: 1~4。

### viewport定义的细微差别

+ 默认视口、理想视口（Default and Ideal Viewports）
+ 可见视口、布局视口（Visual and Layout Viewports）
 ￼￼￼￼￼￼
