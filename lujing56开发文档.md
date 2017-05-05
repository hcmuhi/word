## lujing56编码规范 
  
  <br/>  
**class命名规则**  
  
使用‘-’分割命名  
  
例如：`<div class="body-cont"></div>`  
  
  
  <br/>  
  
**id命名规则**  
  
使用驼峰式命名首字母小写
  
例如：`<div id="bodyCont"></div>`
  
  <br/>  

**js命名规范**
 
变量命名、函数命名，使用驼峰式命名首字母小写

例如：  

    var bodyCont=1; 
    function bodyCont(){}; 
    var bodyCont=function(){}

全局变量命名，使用全大写

例如：`var LOCAL=window;`
  
  <br/>  

**注释规范**

函数需写明用途

例如：

    /**
    * @description 加法运算
    * @param {Num} num1 加数
    * @param {Num} num2 被加数
    * @return {Num} result 结果
    */
    function add(num1,num2`){
        return num1 + num2;
    }


**公共方法使用**

目前提供依赖的js统一放在js/weiget目录下

地址组件使用：

    <!--根据样式绑定，必须添加proCitySelAll，必须添加自定义ID,-->
    <input type="text" class="proCitySelAll"  id="toaddress" />


    <!--城市组件-->
    <script type="text/javascript" src="../../js/weiget/area_yasuo.js" ></script>
    <script type="text/javascript" src="../../js/weiget/areadata-v2.0.js" ></script>
    <script type="text/javascript" src="../../js/weiget/area_plugin.js" ></script>
    <script>
            var area=AddressComponent();
            area.start();
    </script>  

默认组件使用：*(默认所有页面引用)*

    <!--base.js，base提供的基础组件-->
    <!--getJson.js，公共的ajax请求，及alertMsg统一弹窗-->
    <!--template.js，公共的artTemplate模板引擎-->
    <!--ieMode.js，ie低版本提示-->
    <!--iLocalStorage.js，localStorage兼容模式
        iLocalStorage.setItem('key', 'value');
        console.log(iLocalStorage.getItem('key'));
        iLocalStorage.removeItem('key');
    -->
    <!--common.js，公共方法 头部及菜单栏逻辑代码-->
    <!--tf-popup-sp-pc.js，弹窗使用
       new Pop({
            type:"pop",
            content:"网络不给力,请检查网络连接",
             callType:"fail"
        }).init();       
    -->


    <script type="text/javascript" src="../../js/lib/jquery-1.11.3.min.js" ></script>
    <script type="text/javascript" src="../../js/weiget/base.js" ></script>
    <script type="text/javascript" src="../../js/weiget/getJson.js" ></script>
    <script type="text/javascript" src="../../js/lib/template.js"></script>
    <script type="text/javascript" src="../../js/weiget/ieMode.js" ></script>
    <script type="text/javascript" src="../../js/weiget/iLocalStorage.js" ></script>
    <script type="text/javascript" src="../../js/common/common.js"></script>
    <script type="text/javascript" src="../../js/weiget/tf-popup-sp-pc.js" ></script>
    <script type="text/javascript" src="../../js/weiget/tradeFun.js" ></script>
    <script type="text/javascript" src="../../js/common/tradeViewApi.js" ></script>
    <script type="text/javascript" src="../../js/common/partyApi.js" ></script>		
    <script type="text/javascript" src="../../js/weiget/crypto-js.js" ></script>


