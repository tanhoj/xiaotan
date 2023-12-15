<template>
    <div class="outer">
        <div class="box">
        </div>
        <div class="content">
            <h1>到百度首页css3 flex
                
                百度首页设置登录
                网页图片资讯视频贴吧知道文库地图采购更多
                换一换
                热搜榜北京榜
                习近平在越南媒体发表署名文章
                1最高法呼吁取消高额彩礼热
                2新房打折引发老业主不满 多地回应热
                3中国经济在劈波斩浪中坚定前行</h1>
            <p> 4知情人称周海媚还在医院治疗中热
                5销售谈生意时被客户在酒水中下毒
                6小米：余承东发布言论与事实不符
                7女子为8岁女儿寻生父：曾相恋一周
                8深圳平安大厦冒烟着火？假的
                9张家辉：从未阻止妻子关咏荷复出
                10新疆黑脸交警雪地播报路况走红
                11郑爽被强制执行9050万</p>
            <h1>1267岁老人握妻子手买人生第一套房
                13研究发现生两个孩子最有利于长寿
                14新冠变异株JN.1全球加速蔓延
                15谭飞发文辟谣：周海媚并未过世热
                收起工具时间不限所有网页和文件站点内检索
                搜索工具百度为您找到相关结果约12,200,000个
                【CSS3】Flex布局详解_css3 flex-CSDN博客
                2022年10月11日 定义Flex 容器后可以使用相应的属性, 改变子元素的布局方式,让子元素可以自动的挤压或拉伸。 相应属性: 1.justify-content 主轴元素对齐方式2.align-items
                交叉轴元素对齐方式3.fl...
                CSDN博客
                CSS3之flex布局_css3 flex布局-CSDN博客
                2022年12月18日 flex是flexible
                Box的缩写,意思为弹性布局,用来为盒状模型提供最大的灵活性,任何一个容器都可以指定为flex布局-当我们为父盒子设为flex布局后,子元素的float,clear和vertical-alig...
                CSDN博客
                CSS3 flex+多列布局 - 知乎
                2022年11月22日 注意,设为 Flex 布局以后,子元素的float、clear和vertical-align属性将失效。 ​ 2、flex-direction属性 决定主轴的方向(即项目的排列方向)
                flex-direction: row | row-reverse | ...
                知乎</h1>
            <p> 2015年7月10日 flex-basis都设为0,因为flex-grow定义的是,剩余空间分配的比例关系。 | | 大海的子民说: |#|引用 Jasmine说:
                传送门:https://css-tricks.com/snippets/css/a-guide-to-flexbox/ 201...
                www.ruanyifeng.com/blog/2015/0...
                CSS3 中flex 布局
                Flexbox 是 CSS3 中的一种布局模式。它允许元素在一个容器中自动排列,可以使用灵活的方式创建复杂的布局。Flex 布局有很多优点,例如,它很容易实现响应式设计,并且可以很容易地对齐和排列元素。要...
                IT学院</p>
            Flex 布局教程:语法篇 - 阮一峰的网络日志

        </div>
    </div>
</template>
<script>

export default {

}
</script>
<style scoped>
.outer {
    width: 1000px;
    height: 100px;
    border: 1px solid black;
    margin: 20px;
}

.box {
    width: 100px;
    height: 100px;
    background: skyblue;
    animation: to-right2 2s linear 2 2s;
    /*设置动画的名字 动画的时间 匀速（发生动画）发生动画的次数 动画延迟几秒发生*/
}

/* animation和transition的区别：
1.过渡需要触发条件（比如：hover鼠标的触屏）
2.动画可以通过关键帧进行精细的设置 */
/* 动画 （定义关键帧）**/
@keyframes to-right {
    form {
        /* 第一帧 */
    }

    to {
        /* 第二帧 */
        transform: translate(900px);
        background: green;
    }
}

@keyframes to-right2 {
    0% {}

    25% {
        background: red;
    }

    50% {
        background: yellow;
    }

    100% {
        transform: translate(900px) rotate(360deg);
        background: green;
        border-radius: 50%;
    }
}
.content{
    column-count: 3;/* 指定列数 */
    column-gap: 10px;/* 调整列的间距 */
    column-rule: 2px dashed red;/* 调整列的边框 */
}
</style>