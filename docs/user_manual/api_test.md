> 传统的接口自动化测试大多借助第三方测试框架，以代码工程项目的形式实现，不利于管理和维护； MeterSphere 为了解决这个问题，开发了可视化接口自动化测试功能，只需要配置每个接口的入参和 断言，即可实现对接口的自动化测试，同时还开发了基于chrome浏览器的MeterSphere Recorder插件，方便录制场景以及快速导入场景，大大提升了接口测试的效率。

## 首页
> 由测试、报告、测试日历三个部分组成，可快速了解到最近执行的测试内容以及整体的接口测试频次。

- 测试：展示最近 5 次执行的接口测试

- 报告：展示最近 5 次执行的接口测试所生成的报告

- 测试日历：按时间维度展示接口测试执行的频次，颜色越深，代表使用频次越高

![api-home](../img/api/api-home.png)

## 项目
> 对项目进行新增、修改、删除、查询操作

![api-project](../img/api/api-project.png)



### 新增项目
> 点击“创建项目”，录入项目名称和描述

  ![api-project-create](../img/api/api-project-create.png)

  

### 修改项目
> 选择要修改的项目，点击编辑按钮

  ![api-project-edit](../img/api/api-project-edit.png)

  

### 删除项目
> 选择要删除的项目，点击删除按钮

  ![api-project-delete](../img/api/api-project-delete.png)

  

### 查询项目
> 查询全部项目选择“显示全部”，查询单个项目可以根据名称搜索

  ![api-project-search](../img/api/api-project-search.png)

  

## 测试

> 对测试接口或接口集合进行新增、修改、删除、查询操作

### 创建测试
> 点击创建测试，如图 5 步即可成功创建接口测试

  ![api-test-create](../img/api/api-test-create.png)

#### 场景配置
> 场景内的全局变量和请求头配置，作用域为场景内

##### 自定义变量
> 在场景配置中自定义变量的名称和值, 接口运行或者测试集合里面可以通过 ${BASE} 来访问当前场景下定义的全局变量

![api-custom-var](../img/api/api-custom-var.png)

##### 请求头
> 这里增加全局 header，可以在项目中设置全局 header 值

![api-custom-header.](../img/api/api-custom-header.png)

#### 请求配置

##### 请求参数
> 接口 url 的查询字符串

![api-request-parameter](../img/api/api-request-parameter.png)

##### 请求头
> http请求的header，作用域为请求内

![api-request-header](../img/api/api-request-header.png)

##### 请求内容
> http 请求的 body 部分，如果http请求方式是 post, put 等请求方式时会有 请求内容 部分，形式有2种，分别是 键值对（form）、文本（json）

![api-request-content](../img/api/api-request-content.png)


##### 断言
> 断言支持文本、正则和响应时间三种方式，选择断言方式后，点击“+”生成规则即可生效

![api-assert](../img/api/api-assert.png)

##### 提取
> 支持从响应中提取返回值作为变量存储，作用域为场景内，提取方式为正则、JSONPath、XPath三种

![api-extract](../img/api/api-extract.png)


### 修改测试
> 请求执行顺序和场景执行顺序支持拖拽调整；变更结束点击保存

  ![api-test-update](../img/api/api-test-update.gif)


### 删除测试
> 点击测试-显示全部，选择要删除的测试，点击删除按钮

  ![api-test-delete](../img/api/api-test-delete.png)

### 查询测试
> 查询全部测试，点击显示全部，查询单个测试可以根据名称搜索

  ![api-test-select](../img/api/api-test-select.png)

### 执行测试
> 保存成功的测试点击“执行”按钮，编辑完成的测试也可以点击“保存并执行”按钮，页面将会跳转到当前测试的测试报告中。

  ![api-test-execute](../img/api/api-test-execute.png)

  ![api-test-execute1](../img/api/api-test-execute1.png)

### 更多操作
> 创建性能测试，接口测试保存后可以直接创建该场景对应的性能测试，配置压力测试参数后，可一键执行

![api-test-more-operations](../img/api/api-test-more-operations.png)

![api-test-more-operations1](../img/api/api-test-more-operations1.png)

## 报告

> 对接口测试报告的查询和删除操作

### 查询报告

> 查询全部报告，点击显示全部，查询单个报告可以根据名称搜索

![api-report-selectAll](../img/api/api-report-selectAll.png)

### 报告详情

> 展示接口测试的执行结果，包含响应时间、错误、断言以及请求的具体响应报文等

![api-report-detail](../img/api/api-report-detail.png)

![api-report-detail1](../img/api/api-report-detail1.png)

![api-report-detail2.](../img/api/api-report-detail2.png)

### 删除报告

> 点击报告-显示全部，选择要删除的报告，点击删除按钮

![api-report-delete](../img/api/api-report-delete.png)





