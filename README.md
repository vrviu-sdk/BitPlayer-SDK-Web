# BitPlayer-SDK-Web

[![](https://img.shields.io/badge/Powered%20by-vrviu.com-brightgreen.svg)](https://vrviu.com)

## 版本历史
 20180517   V1.0   支持主流浏览器和微信内的H5播放，支持全屏模式和VR模式；  
 
## 产品特点
**1. VR视频格式**：支持 **180度3D/360度2D/360度3D** 

**2. 音视频编码**：H.264, AAC  

**3. 最大分辨率**：4K

**4. 播放格式**：点播，直播

**5. 编码方式**：除了支持标准算法的编码方式，还支持VRVIU-FE算法，带宽节省高达50%

**6. 播放模式**：全屏模式/VR模式；

**7. 播放操作**：  
-- 支持视频播放/暂停；  
 支持手势拖拽和陀螺仪旋转操作；  
 支持进度条的点击或拖拽；  
 支持视角位置和一键还原到主视角功能；  

**8. 播放平台**：支持微信/QQ/Chrome/Safari等平台播放

## 效果预览以及操作说明
**1.  视频封面，展示公司logo及视频简要介绍**  
-支持360度全景封面图、2D封面图  
-支持陀螺仪旋转和手势拖拽操作  
-支持视角位置和一键还原到主视角功能（点击右侧小圆圈）  

![](https://github.com/vrviu-sdk/VRVIU-BitPlayer-Demo-Web/blob/master/img/11.png)

**2.  点击播放按钮，全屏模式播放视频**
-	支持视频播放/暂停
-	支持手势拖拽和陀螺仪旋转操作 
-	支持进度条的点击或拖拽
-	支持视角位置和一键还原到主视角功能（点击右侧小圆圈）
-	点击VR眼镜按钮可以切换到VR模式

![](https://github.com/vrviu-sdk/VRVIU-BitPlayer-Demo-Web/blob/master/img/12.png)

**3.  进入VR模式播放**
- 支持VR模式切换提示框
-	支持返回全屏观看模式
-	支持市场主流的大部分基于Google Cardboard谷歌VR纸盒的头戴设备
- 支持设置Cardboard版本和参数调整（已经优化参数，不建议修改）

![](https://github.com/vrviu-sdk/VRVIU-BitPlayer-Demo-Web/blob/master/img/13.png)

## Demo展示

**标准算法编码**：https://rs1-pv.vrviu.com/h5/v1.2/index.html 

**VRVIU-FE编码**：https://rs1-pv.vrviu.com/h5/v1.2/index.html?algorithm=1&format_degree=360&domain=https://rs1-pv.vrviu.com/1min/
 

## 导入SDK
### 1. 开发准备
下载最新的VRVIU_BitPlayer.min.js以及VRVIU_BitPlayer.min.css

### 2. 导入SDK
##### 2.1 新建Html文件导入js-sdk以及css文件
```html
<!DOCTYPE html>
<html lang="en">
<head>
        <meta charset="utf-8">
        <title></title>
        <meta name="description">
        <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
        <meta name="apple-touch-fullscreen" content="yes">
        <meta name="x5-fullscreen" content="true">
        <meta name="x5-page-mode" content="app">  
        <meta name="full-screen" content="yes">
        <meta name="format-detection" content="telephone=no">
        <meta name="apple-mobile-web-app-capable" content="yes">
        <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent" />
        <title></title>
        <link rel="stylesheet" href="https://vm.vrviu.com/css/h5/v1.2/VRVIU_BitPlayer.min.css">
        <script src="https://vm.vrviu.com/js/h5/v1.2/VRVIU_BitPlayer.min.js"></script>
</head>
<body>

</body>
</html>
```

##### 2.2 配置工程权限
引入新建js文件配置相关参数及权限

```javascript
<script src="./dest/ready/js/BitPlayer_Configure.min.js"></script>

//BitPlayer_Configure.min.js

new VRVIU_BitPlayer({
        src:"https://rs1-pi.vrviu.com/h5/thumb/video/viu6ire0r/viu6ire0r.200000000013.0.jpg",
        url:"https://rs1-pv.vrviu.com/viu6ire0r/viu6ire0r.200000000013.0.mp4",
        format_degree:"360",
        AppId :'vrviu_altsdk',
        AccessKeyId :'730c029686b86a332facca0bb1a9f53a',
        AccessKeySecret:"14d90ef1ee2be9f6c3469f46e2a3e566",
        BizId :'altsdk_web_demo'
})
```




## 配置参数表
 |参数|说明|是否必填|类型|
 |:---|:---|:---|:---|
 |src|首页360度图片url地址，不填时将展示黑色的背景。|非必填|String|
 |url|视频文件存放在服务器上的地址。|必填|Object|
 |format_degree|视频视角分类，目前只支持360度视频、180度视频。|必填|String|
 |AppId|分配给用户的ID，可通过 www.vrviu.com 填写表单或者联系客服申请。|必填|String|
 |AccessKeyId|分配给用户的ID，可通过 www.vrviu.com 填写表单或者联系客服申请。|必填|String|
 |BizId|分配给用户的ID，可通过 www.vrviu.com 填写表单或者联系客服申请。|必填|String|
 |AccessKeySecret|分配给用户的ID，可通过 www.vrviu.com 填写表单或者联系客服申请。|必填|String

## 联系我们
 如果有技术问题咨询，请加入官方QQ群：136562408  
 商务合作请电话：0755-86960615；邮箱：business@vrviu.com；或者至[官网](http://www.vrviu.com)"联系我们"。  
