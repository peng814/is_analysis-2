# 实验1：业务流程建模（老师示范）
|学号|班级|姓名|照片|
|:-------:|:-------------: | :----------:|:---:|
|201510414108|软件(本)15-1|郭昆进|![flow1](../head.jpg)|

## 流程图1：考试及成绩管理流程

**PlantUML源码如下：**

``` flow1
@startuml
title 期末考试流程
start
:安排考试;
:考试安排表]
:出卷;
fork
:A、B试卷]
fork again
:打印审批表]
:审批签字;
:打印审批表]
end fork
:打印试卷;
:试卷]
:参加考试;
:答卷]
:阅卷出成绩;
fork
:成绩单]
if(有不及格?) then(有)
:安排补考;
endif
:补考安排表]
fork again
:答卷]
:装订存档;
end fork
:期末流程结束;

stop

@enduml
```

**业务流程图如下：**

![flow1](aaa.png)

**流程说明：**

说明文字....

## 流程图2： 客户维修服务流程

**PlantUML源码如下：**

``` flow2
@startuml
start
if (Graphviz installed?) then (yes)
:process all\ndiagrams;
else (no)
:process only
__sequence__ and __activity__ diagrams;
endif
stop
@enduml
```

**业务流程图如下：**

![flow2](flow2.jpg)

**流程说明：**

说明文字....
