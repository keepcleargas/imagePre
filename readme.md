## 插件描述
一个简单的图片预览jquery 插件.

##使用方法

<!-- code -->
        <div class="imagePre" data-provides="imagePre">
            <div class="thumbnail" style="width:160px;height:120px;">
                    <img class="imagePreview" src="data:image/gif;base64,R0lGODlhAQABAIAAAP///////yH5BAEKAAEALAAAAAABAAEAAAICTAEAOw=="/>
            </div>
            <span class="btn btn-file"><span class="imagePre-new">选择图片</span><span
                            class="imagePre-exists">修改</span>
            <input type="file" class="input-file"/></span>
            <span data-dismiss="imagePre" class="btn imagePre-exists">删除</span>
        </div>

js调用:
<!-- code -->
        $(document).ready(function () {
            $('div.imagePre').imagePre({'name':'sampleImage','checkBoxName':'isSampleNull'});
            //name 为文件输入的字段的名称, checkboxName即是否删除图片的字段名称
        });

##和bootstrap fileupload区别.

1. 从bootstrap fileupload中 去除了 文件的上传支持
2. 增加了图片删除的 操作,即 添加 一个checkbox字段((':input').name+'_isRemoved')，去判断是否删除已有的图片.而这点恰是bootstrap fileupload没支持的.

##参考来源
bootstrap fileupload:[http://jasny.github.com/bootstrap/javascript.html#fileupload](http://jasny.github.com/bootstrap/javascript.html#fileupload)

