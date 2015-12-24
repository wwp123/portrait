#头像上传插件
 
####官方地址：http://fex.baidu.com/webuploader/

##兼容性

* ie9+


##样例：

###1、使用步骤
* 引入样式文件

```javascript
<link href="style/jquery.Jcrop.css" rel="stylesheet" type="text/css" />
<link href="style/new.less" rel="stylesheet" type="text/less" />
```
* 引入js文件

```javascript
<script src="javascript/less-1.7.3.min.js"></script>
<script src="javascript/jquery-2.1.3.js" type="text/javascript" charset="utf8"></script>
<script src="javascript/jquery.Jcrop.js" type="text/javascript" charset="utf8"></script>
<script src="javascript/webuploader.min.js" type="text/javascript" charset="utf8"></script>
<script src="javascript/modPicture-old.js" type="text/javascript" charset="utf8"></script>
<script src="javascript/foundation.min.js" type="text/javascript" charset="utf8"></script>
<script src="javascript/tab.exam.js"></script>
```
 

* 在页面上添加代码

```javascript

<div class="photo-main-righ" id="frame_main_rig1_r1_t2">
<div class="photo-upload margin-t">
    <div class="row">
        <div class="small-12 columns">
            <div class="tab-rec-1">
                <div class="tab clearfix no-margin">
                    <ul class="clearfix" id="datatable_tab">
                        <li class="on">
                            <div class="tl">
                                <div class="tr">
                                    <div class="tc"><a href="#" target="_blank">自定义头像</a></div>
                                </div>
                            </div>
                        </li>
                        <li>
                            <div class="tl">
                                <div class="tr">
                                    <div class="tc"><a href="#" target="_blank">热门推荐头像</a></div>
                                </div>
                            </div>
                        </li>
                        
                    </ul>
                </div>
                <div>
                <div class="modcon clearfix padding-t10">
                    <div class="row">
                        <div class="small-12 medium-12 large-12 columns padding-r">
                            <div id="data_dttab_con_1" class="clearfix" style="display: block;">
                                <div class="small-12 medium-6 large-6 columns padding-r">
                                    <div class="modPic" id="modPic">
                                        <div class="uploader-area" id="filePicker">点击选择图片</div>
                                        <div class="uploader-list" id="fileList"></div>
                                   </div>
                                    <div class="padding-b50 small-padding-t">
                                            <a class="button radius secondary small right" id="filePicker2" style="display:none;"><i class="fa fa-upload fa-fw font9"></i>重新上传</a>
                                            <!--<a class="button radius secondary small right" id="rotate-img" style="display:none;"><i class="fa fa-repeat fa-fw font9"></i>90度旋转</a>-->
                                            <a class="button padding-l30 padding-r30 radius save-load">保存</a>
      </div>
                                 </div>
                                 <div class="small-12 medium-6 large-6 columns">
                            <div class="preview-pic">
                            <div class="mar-bom-15 padding-b30">
                                <h5>效果预览</h5>
                                <p>你上传的图片会自动生成3种尺寸，请注意小尺寸的头像是否清晰。</p>
                                <p>建议使用正方形图片，支持PNG、GIF、JPGE格式。</p>
                            </div>
                            <div class="row">
                                <div class="small-12 medium-8 large-8 columns">
                                    <div class="crop crop1 margin-b left padding-r50" id="crop1">
                                <div class="crop-img crop-img1"><img/></div>
                                <p class="padding-l20 hide">大尺寸头像，180*180像素</p>
                            </div>
                                </div>
                                <div class="small-12 medium-4 large-4 columns">
                                    <div class="row">
                                        <div class="small-6 medium-12 large-12 columns">
                                            <div class="crop crop2 margin-b left" id="crop2">
                                                <div class="crop-img crop-img2"><img /></div>
                                                <p class="hide" style="width:80px;">中尺寸头像，60*60像素（自动生成）</p>
                                            </div>
                                        </div>    
                                        <div class="small-6 medium-12 large-12 columns">
                                            <div class="crop crop3 margin-b left" id="crop3">
                                                <div class="crop-img crop-img3 margin-l15"><img/></div>
                                                <p class="hide" style="width:80px;">小尺寸头像，30*30像素（自动生成）</p>
                                            </div>
                                        </div>	
                                    </div>	
                                </div>	
                            </div>	
                        </div>	
                        </div>
                                </div>
                            <div id="data_dttab_con_2" style="display:none;">
                                <div class="small-12 medium-6 large-6 columns padding-r">
                                    <div class="info_list_2 clearfix">
                                    <div class="pass-portrait-tabcontent margin-t10">
                                       <ul class="pass-portrait-hotrecommend clearfix">
                                        <li class="tupian">
                                        <img src="images/13275477_116x86_0.jpg" data-th-src="|${tempPath}images/13275477_116x86_0.jpg|"/>
                                        </li>
                                        <li class="tupian">
                                        <img src="images/star-black-128.png" data-th-src="|${tempPath}images/star-black-128.png|"/>
                                        </li>
                                        </ul>
                                    </div>
                                    
                                    </div>
                                </div>
                                <div class="small-12 medium-6 large-6 columns">
                            <div class="preview-pic">
                            <div class="mar-bom-15 padding-b30">
                                <h5>效果预览</h5>
                                <p>你上传的图片会自动生成3种尺寸，请注意小尺寸的头像是否清晰。</p>
                                <p>建议使用正方形图片，支持PNG、GIF、JPGE格式。</p>
                            </div>
                            <div class="row">
                                <div class="small-12 medium-8 large-8 columns">
                                    <div class="crop-2 crop1 margin-b left padding-r50" id="crop1">
                                <div class="crop-img-2 crop-img1"><img /></div>
                                <p class="padding-l20 hide">大尺寸头像，180*180像素</p>
                            </div>
                                </div>
                                <div class="small-12 medium-4 large-4 columns">
                                    <div class="row">
                                        <div class="small-6 medium-12 large-12 columns">
                                            <div class="crop-2 crop2 margin-b left" id="crop2">
                                                <div class="crop-img-2 crop-img2"><img /></div>
                                                <p class="hide" style="width:80px;">中尺寸头像，60*60像素（自动生成）</p>
                                            </div>
                                        </div>	
                                        <div class="small-6 medium-12 large-12 columns">
                                            <div class="crop-2 crop3 margin-b left" id="crop3">
                                                <div class="crop-img-2 crop-img3 margin-l15"><img /></div>
                                                <p class="hide" style="width:80px;">小尺寸头像，30*30像素（自动生成）</p>
                                            </div>
                                        </div>	
                                    </div>	
                                </div>	
                            </div>	
                        </div>	
                        </div>
                            </div>
                        </div>
                        <div class="large-12 medium-12 small-12 columns">
                            <!--<a class="button padding-l30 padding-r30 radius save-load">保存</a>-->
                      </div> 
                        <div class="row posi-rela hide">
                         <div class="large-12 medium-12 small-12 columns">
                                <img src="images/loading-017.gif"/>
                                <span class=" font-large padding-l10">请稍候，头像上传中...</span>
                          </div> 
                        </div>
                        <!--操作成功提示框-->
                        <div class="fixed" id="reveal3-2">
                            <div class="row">
                                <div class="large-12 columns" id="operate_alert_into">
                                    <div data-alert="" class="success alert-box warning  nomarg v_show_oper_info">
                                        <div><i class="fa fa-fw fa-check"></i><span class="v_show_info3">保存成功.</span></div>
                                    </div>
                                </div>
                            </div>
                        </div> 
                        
                    </div>
                </div>
            </div>
        </div>
      </div>
</div>

</div>
</div>
    
```
###2、demo
* http:http://192.168.14.97:8080/acc/wwp/portrait/

##方法和API
###1、方法
     无
     
###2、参数说明
     无
        

