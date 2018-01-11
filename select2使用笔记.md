Select2是一款基于Jquery的下拉选择器,支持搜索,远程调用,分页...官网文档:https://select2.org/

    引用select2(css)样式和js:
    <link href="select2/css/select2.min.css" rel="stylesheet" />
    <script src="select2/js/select2.min.js"></script>
1.初始化select2选择器:

    $("#myselect2").select2({
       //异步方法调用
        ajax: {
           url: "http://example.org/api/test",
           cache: false
         }
    });
2.select2中的disable属性(和jquery一样)

    //禁用
    $("#myslect2").prop("disabled", false);
    //启用
    $("#myslect2").prop("disabled", true);
