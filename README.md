# colResizable
### 增加了双击表头展开此列的方法。
### 为和datatables兼容，datatables加scrollY属性列表tbody拖不动，去掉此属性就好。

**使用方法：**
 $('#dbBackupList').colResizable({
    "useDatableId": "dbBackupList", //必填,table id名
    "wrapClass": "wtable",  //选填，table外层div，拖动或双击展开列时长度不够外层出现滚动条
    "disabledColumns":[0]   //选填，禁止双击拖拽的列
 });
### 增加tableResize方法：列表开始隐藏后再显示时，可拖动的位置和table表头的位置对不上，调用此方法重写可拖动表头位置。
**使用方法：**
 $('#dbBackupList').tableResize({"useDatableId": "dbBackupList" //必填,table id名})
 
