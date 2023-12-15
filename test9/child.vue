<template>
    <div>
        <div class="box">
            <div class="box-item"><span class="box1">阿酷</span><h1>aaa</h1></div>
            <div class="box-item2"><div class="box2">第二个</div></div>
            <div class="box-item3"><div class="box3">我是老三</div><h3>ccc</h3></div>
            <div class="com box4"></div>
            <div class="com box5"></div>
            <div class="com box6"></div>
   
           
            <div class="left">
                shanhguishanhguishanhguishanhguishanhguishanhguishanhguishanhguishanhguishanhguishanhguishanhguishanhguishanhguishanhguishanhguishanhguishanhguishanhguishanhguishanhguishanhguishanhguishanhgui
            </div>
            <div class="right">阿酷</div>
        </div>
        <div>
            <input list="data">
            <datalist id="data">
                <option value="a1"></option>
                <option value="b2b"></option>
                <option value="c1"></option>
            </datalist>
            <details style="text-align: center;">
                <summary>
                    如何
                </summary>
                <p>222</p>
            </details>
            <ruby>
                <p>a<mark style="color: red;">ccc</mark>bbbbaa</p>
                <rt>chi</rt>
            </ruby>
        </div>
    </div>
</template>
<script>

var fsr = document.documentElement.clientWidth;
if (fsr > 1600) {
    fsr = 1600;
}
document.getElementsByTagName("html")[0].style.fontSize = 10 * (fsr / 1600) + 'px'

export default {
    data() {
        return {
            stus: ['巧克力', '小猫', '猿']
        }
    }
}
</script>
<style scoped>
@font-face {
  font-family: "阿里";font-weight: 400;src: url("//at.alicdn.com/wf/webfont/U2Vzq4CGMotq/JTPSNv71Ay9A.woff2") format("woff2"),
  url("//at.alicdn.com/wf/webfont/U2Vzq4CGMotq/zNtnKrNp6YoS.woff") format("woff");
  font-display: swap;
}
.left {
    font-size: 2rem;
    width: 200px;
    background: green;
    flex: 0 0 200px;
    text-shadow: 0 0 2rem red; /* 文本阴影 水平位移 垂直位移 模糊程度 阴影颜色 */
    white-space: wrap;
    text-overflow: ellipsis;
    overflow: hidden;
    text-decoration: overline;
    font-family: "阿里";
}

.right {
    font-size: 5rem;
    width: 200px;
    background: gold;
    font-family: "阿里";
    
}


.box {
    background: gray;
    width: 100%;
    height: 500px;
    display: flex;
}

.box-item {
    width: 22rem;
    height: 22rem;
    background: rgb(215, 175, 175);
    font-size: 2rem;
    margin: .5rem;
    flex: 1;
    font-size: 2rem;
    text-decoration: overline dashed blue;  /* 让文本在上方有一条蓝色的虚线 */
}
.box-item2 {
    width: 22rem;
    height: 22rem;
    background: rgb(96, 196, 119);
    font-size: 2rem;
    margin: .5rem;
    flex: 1;
    font-size: 2rem;
    transform-style: preserve-3d ;/* 开启3D空间  想要实现3D变换，就要给盒子的父亲开启3D空间*/
    perspective: 300px;/* 设置景深 就是视觉看的效果的远近*/
    perspective-origin: 12rem 12rem;/* 设置观看时自己所在的位置 */
    font-family: "阿里";
}
.box-item3 {
    width: 22rem;
    height: 22rem;
    background: rgb(12, 123, 38);
    font-size: 2rem;
    margin: .5rem;
    flex: 1;
    font-size: 3rem;
}
.box1{
    width: 9rem;
    height: 9rem;
    background-image:linear-gradient(red,green,yellow);  /* 线形渐变liner 径向渐变radial */
        /* 2D变换 */
    /* transform: translate(20px); 位移*/
    /* transform: scale(1.5); 缩放*/
    /* transform: rotate(29deg); 旋转*/
    transform: translate(50px,29px) scale(1.2) rotate(30deg);  /* 多重2D变换 */
    transform-origin: 50px 50px;  /* 切换原点  就是按照原点这一个点进行一系列的位移、缩放等变换*/
    display: inline-block; /* 行内快元素  让span变成块元素,就可以使用transform */
}
.box2{
    width: 10rem;
    height: 10rem;
    border: 1px solid black;
    background-color: skyblue;
    /* 3D变换 */
    /* transform: scaleZ(0.5); */
    /* transform: translateZ(200px);*/
    /* transform: rotateY(20deg); */
    transform: translateZ(20px) scaleZ(1) rotateY(30deg);/* 多重3D变换 */ 
}
.box3{
    width: 10rem;
    height: 10rem;
    border: 1px solid black;
    background-color: rgb(214, 100, 176);
    transition: height,width,opacity 1s;/* 设置需要过渡的宽、高、透明度  设置过渡需要的时间 */
    transition: all 1s;/* 设置能过度的属性，都进行过渡 */
}
.box3:hover{
    width: 12rem;
    height: 12rem;
    opacity: 0.5;
    transform: rotate(20deg);
}
.com{
    width: 20rem;
    height: 20rem;
    transition: all 3s;
}
.box4{
    background: red;
}
.box5{
    background: green;
}
.box6{
    background: yellow;
}
.box .com:hover{
      width: 25rem;
}
</style>