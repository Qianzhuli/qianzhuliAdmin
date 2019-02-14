### 代码整体
1.  使用git版本控制
2.  yii2框架
3.  cmder.net远程链接

------------

### 整体结构

1. 前端展示：网贷评级+论坛部分
2. 管理后台：对评级平台的展示，对论坛部分发布的控制，以及用户管理
3. 数据库：对前端展示提供接口+对管理后台增删改查

------------

### 操作记录
1. 进行url美化：在frontend/config/main.php中添加路由规则+frontend/web/.htacess文件
2. 独立的用户系统：会员表，管理表
3. 语言包配置：
  - 在frontend/config/main.php中添加语言包配置'language' => 'zh-CN', 'common' => 'common.php',
 - 新建messages->zh-CN->common.php view视图使用Yii::t('yii','Home')---yii自带 Yii::t('common','About') ---自定义
 - 使用其他语言包可用test.php进行其他设置

#### 增加功能点

    editor.md/
    1. 后台添加文章审核功能 后台把is_vaild字段为0的审核通过，即update改成1
    2. 用户管理系统优化     

```html
<!-- English -->
<script src="../dist/js/languages/en.js"></script>

<!-- 繁體中文 -->
<script src="../dist/js/languages/zh-tw.js"></script>
```
