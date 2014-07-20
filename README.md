# jquery-upload [![spm version](http://spmjs.io/badge/jquery-upload)](http://spmjs.io/package/jquery-upload)

AUTHOR WEBSITE: [http://ydr.me/](http://ydr.me/)

jquery.fn.upload 单个上传、批量上传、二进制上传

**五星提示：当前脚本未作优化、未完工，请勿用在生产环境**

__IT IS [A SPM PACKAGE](http://spmjs.io/package/jquery-upload).__





#USAGE
```
var $ = require('jquery');
require('jquery-upload')($);


// 普通 input:file
$('#demo').upload();

// 二进制
$('#demo').upload('blob', blob);
```



#OPTIONS
```
$.fn.upload.defaults = {
    // 留空表示提交到当前页面
    action: "",
    // 头信息
    headers: {},
    // 传递额外数据（键值对字符串）
    data: null,
    // 留空表示默认读取表单文件的name值
    name: "",
    // 完成回调，无论成功还是失败
    oncomplete: $.noop,
    // 成功回调
    onsuccess: $.noop,
    // 失败回调
    onerror: $.noop,
    // 进度回调
    onprogress: $.noop
};
```
