# Temperature Rise/温升   
  
## 基本信息
基本信息如下：  
* 文件编号：OLDF-1607   
* 版本：V0.0.1   
* 版本别名：2018-05   
* 版本状态：编辑中   
* 简介：温升数据格式规范。    
  
  
## 文件要求  
支持格式：CSV、JSON  

## 格式规范-CSV  
基本格式要求如下：  
* 第一行为标题；  
* 第一行标题依次为：序号、时间、数据点1、数据点2、......、数据点N  
* 从第二行开始录入数据
 

## 格式规范-JSON  
JSON格式如下：
{
  "oldf" : "OLDF-1607",
  "version" : "V0.0.1",
  "format" : {
    "pointList" : [
      {
        name : "Enclosure outside",
        nameZh : "外壳外壁温度",
        pointDataPosition : 1
      },
      {
        name : "Enclosure inside",
        nameZh : "外壳内壁温度",
        pointDataPosition : 2
      },
      {
        name : "Lamp base",
        nameZh : "保险丝温度",
        pointDataPosition : 3
      }
    ]
  }
  data : {
   year : "2018",
   list : [
     {
       "date" : "04-14 14:23:29",
       pointList : [22.6, 22.5, 22.3]
     },
     {
       "date" : "04-14 14:28:29",
       pointList : [22.6, 22.5, 22.3]
     }
   ] 
  }
}

## 附录A-时间格式规范  
TODO
