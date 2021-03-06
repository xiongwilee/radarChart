# 花式雷达图

<img width="40%" src="https://github.com/xiongwilee/radarChart/blob/master/demo.png?raw=true" />

### 示例

[http://wilee.me/radarChart/](http://wilee.me/radarChart/)


### 使用方法

**一、引入依赖，在html中定义容器：**

```html
<script type="text/javascript" src="radarChart.js"></script>
<!--容器的大小就为雷达图canvas的大小-->
<div id="radar" style="width:400px;height:400px;"></div>
```

**二、实例化**

```javascript
    const element = document.getElementById('radar');
    
    // 数据格式
    const DATA = {
      list: [{
        name: '学生学习',
        ringColor: '#28b447',
        ringBgColor: '#eaf9f0',
        data: [{
          name: '学习准备',
          value: 80
        }, {
          name: '倾听',
          value: 90
        }, {
          name: '学生互动',
          value: 100
        }, {
          name: '自主学习',
          value: 90
        }, {
          name: '目标达成',
          value: 50
        }]
      },{
        name: '教师教学',
        ringColor: '#e43633',
        ringBgColor: '#feeaf0',
        data: [{
          name: '教学环节',
          value: 40
        }, {
          name: '教学行为',
          value: 100
        }, {
          name: '指导学习',
          value: 100
        }, {
          name: '教学机制',
          value: 80
        }, {
          name: '教学特质',
          value: 70
        }]
      }, {
        name: '课程性质',
        ringColor: '#2595d5',
        ringBgColor: '#eaf3f7',
        data: [{
          name: '目标',
          value: 60
        }, {
          name: '内容',
          value: 40
        }, {
          name: '实施',
          value: 90
        }, {
          name: '评价',
          value: 100
        }, {
          name: '资源',
          value: 20
        }]
      }, {
        name: '课堂文化',
        ringColor: '#772094',
        ringBgColor: '#f3e6f3',
        data: [{
          name: '思考',
          value: 80
        }, {
          name: '民主',
          value: 60
        }, {
          name: '创新',
          value: 70
        }, {
          name: '关怀',
          value: 60
        }]
      }]
    };

    radarChart(element, DATA);
```

### 贡献&反馈

欢迎提issue、fork，有任何疑问也可以邮件联系：xiongwilee[at]foxmail.com。