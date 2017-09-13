#响应式web设计

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
 
