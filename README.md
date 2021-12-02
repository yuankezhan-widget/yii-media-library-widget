# yii2-widget-media-library

#### 介绍
yii widget 媒体库

#### 安装教程

1.  composer require yuankezhan/yii-tiny-editor-widget


#### 使用说明


```
<?php

use yii\helpers\Url;
use yuankezhan\mediaLibrary\MediaLibrary; ?>

<button class="showImgBox">测试</button>

<?= MediaLibrary::widget()?>
<script>
    var editorMediaUpload = new mediaLibrary().init({
        imgListUrl : "<?=$mediaConfig['imgListUrl']?>",
        groupListUrl : "<?=$mediaConfig['groupListUrl']?>",
        addImgUrl : "<?=$mediaConfig['addImgUrl']?>",
        addGroupUrl : "<?=$mediaConfig['addGroupUrl']?>",
        sureCallback : "addImg",
    });

    editorMediaUpload.showBox();
</script>

```

![输入图片说明](https://images.gitee.com/uploads/images/2021/1112/171317_678964e4_782530.png "img.png")