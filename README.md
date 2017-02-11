# ajaxfileupload

Improved [carlcarl/AjaxFileUpload](https://github.com/carlcarl/AjaxFileUpload) and fixed some bugs.

[![Latest Stable Version](https://poser.pugx.org/yongtiger/js-js-ajaxfileupload/v/stable)](https://packagist.org/packages/yongtiger/js-ajaxfileupload)
[![Total Downloads](https://poser.pugx.org/yongtiger/js-ajaxfileupload/downloads)](https://packagist.org/packages/yongtiger/js-ajaxfileupload) 
[![Latest Unstable Version](https://poser.pugx.org/yongtiger/js-ajaxfileupload/v/unstable)](https://packagist.org/packages/yongtiger/js-ajaxfileupload)
[![License](https://poser.pugx.org/yongtiger/js-ajaxfileupload/license)](https://packagist.org/packages/yongtiger/js-ajaxfileupload)


## Features

- add `handleError`
- add `start` and `beforeSend` local callbacks of events
- fix ie9 and ie 10
- fix bugs: confict with yii.js(350)


## Example:

```js
ajaxFileUpload: function () {
    $.ajaxFileUpload({url: '<your url>', 
        secureuri: false,
        fileElementId:'<your file element id>',
        type: 'post',
        data: '<your data>',
        dataType: 'json',

        start: function () {
            // ...
        },

        beforeSend: function () {
            // ...
        },

        success: function (data, status) {
            // ...
        },

        error: function (XMLHttpRequest, textStatus, errorThrown) {
            // ...
        },

        complete: function () {
            // ...
        }
    });
},
```


## References

* https://github.com/carlcarl/AjaxFileUpload
* http://www.cnblogs.com/zrp2013/archive/2013/05/29/3106435.html
* http://www.oschina.net/question/1246890_142999
* http://www.developwebapp.com/5538869/
* http://www.lai18.com/content/9621987.html

## License 
**ajaxfileupload** is released under the MIT license, see [LICENSE](https://opensource.org/licenses/MIT) file for details.