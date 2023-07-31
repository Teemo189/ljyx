数据采集
=====================


.. raw:: html

 <h4><b>项目管理</b></h4>
 <p style="text-indent:2em;text-align:justify;">在项目管理页面中可对一个项目进行增删改查操作，项目名称不可重复，删除项目时会删除其中包含的所有路线与病害数据，切勿轻易删除。一个项目采集完成后需将项目状态编辑为已采集。操作栏中点击进入可进入路线管理页面。</p>
 <h4><b>路线管理</b></h4>
 <p style="text-indent:2em;text-align:justify;">在路线管理页面中可对一个项目进行增删改操作，路线名称不可重复，开始桩号格式为K0000+000，桩号增减选项与行进方向选项互不关联。一条路线采集完成后需将路线检测状态编辑为结束检测。删除路线时会删除其中所有的病害数据，切勿轻易删除。操作栏中点击进入可进入该路线的病害检测页面。</p>
 <h4><b>病害录入</b></h4>
 <p style="text-indent:2em;text-align:justify;padding: 0;margin: 0;">进入病害检测页面时，若未在导航页授权GPS，在此处仍可继续授权。授权后，会提示是否开始检测，若不选择开始，则无法录入病害。选择开始后会开始检测。</p>
 <p style="text-indent:2em;text-align:justify;">页面上方是病害检测的信息栏，可以实时看到当前检测的一些数据信息，如<a href="#image1">图1</a>。对病害检测信息栏中个名词解释如下：</p>

 <link rel="stylesheet" type="text/css" href="./_static/viewer.min.css"/>
 <script src="./_static/viewer.min.js" type="text/javascript" charset="utf-8"></script>
 <div><img id="image1" src="./_static/1.png" alt="Picture"></div>
 <p style="color: dimgray;text-align: center;">图1  信息栏</p>
 <script type="text/javascript">var viewer = new Viewer(document.getElementById('image1'));</script>

 <ul>
 <li><b>当前状态</b>：指该路线目前的检测状态，包括未开始、正在检测和暂停。</li>
 <li><b>病害记录</b>：指该路线所有的病害数。</li>
 <li><b>照片记录</b>：指该路线所有的照片数。</li>
 <li><b>起点桩号</b>：指开始检测路线的第一个桩号，即创建路线时输入的桩号。</li>
 <li><b>上次校对桩号</b>：上一次校对桩号时产生的桩号，若无则与起点桩号相同。</li>
 <li><b>上次校对时间</b>：上一次产生桩号时的时间。</li>
 <li><b>累计距离</b>：该路线已检测的总距离。</li>
 <li><b>本次距离</b>：从上次校对桩号位置到当前位置的距离。</li>
 <li><b>校对次数</b>：用户检测该路线校对桩号的总次数。</li>
 <li><b>GPS</b>：当前卫星定位坐标，每5秒更新一次。</li>
 <li><b>运行时间</b>：从开始到现在的时间。</li>
 <li><b>标线</b>：标线缺失采集的状态，未进行中会显示未采集，进行中会显示已采集长度。</li>
 <li><b>路缘石</b>：路缘石缺失采集的状态，未进行中会显示未采集，进行中会显示已采集长度。</li>
 <li style="text-align:justify;"><b>当前桩号</b>：即设备所处位置的预估桩号（略有波动，最好稳定后取值），右下角文字表示道路的行进方向和桩号的增减。</li>
 <li style="text-align:justify;"><b>整公里校对</b>：点击该按钮会进行一次桩号校对，但校对方式为桩号后三位小于500则清零，比如K0023+350则变为K0023+000；大于等于500则清零且公里数加1，比如K0023+750则变为K0024+000。</li>
 </ul>
 <p style="text-indent:2em;text-align:justify;">页面下方是8个页面的组合，包括检测状态、三个大类的病害录入页面和两个特殊病害录入页面、病害列表页面、桩号校对页面。各页面的具体操作方法以及注意事宜如下：</p>
 
 <h6><b>①检测状态</b></h6>
 <p style="text-indent:2em;text-align:justify;">该页面主要功能是开启、暂停、继续或结束检测；并可以开启或关闭GPS信号，修改GPS定位的频率，如<a href="#image2">图2</a>；同时可以在该页面查看病害轨迹图。若进入页面未开始检测，也可以手动在该页面开始检测，开始检测后可以暂停和结束。轨迹图效果就是每存入一个病害就会在轨迹上产生一个轨迹点，横竖坐标是使用的GPS坐标，轨迹图可以放大缩小。</p>
 <div><img id="image2" src="./_static/2.png" alt="Picture"></div>
 <p style="color: dimgray;text-align: center;">图2  检测状态</p>
 <script type="text/javascript">var viewer = new Viewer(document.getElementById('image2'));</script>
 
 <h6><b>②路基检测、沿线设施、集团参数</b></h6>
 <p style="text-indent:2em;text-align:justify;">这三个页面主要是用于病害的录入。每个大类里面又包含不同的二级病害，如<a href="#image3">图3</a>。</p>
 <div><img id="image3" src="./_static/3.png" alt="Picture"></div>
 <p style="color: dimgray;text-align: center;">图3  普通病害录入</p>
 <script type="text/javascript">var viewer = new Viewer(document.getElementById('image3'));</script>
 <p style="text-indent:2em;text-align:justify;">发现病害后，先选择二类病害，然后确定实时的桩号，选择桩号时可以进行刷新。再次选择三类病害或默认的二类病害，再输入病害的数据量。桩号、病害类型（三级）与病害数据量为必填项。然后选择严重程度或是让系统自动判断严重程度。最后用户可以选择拍照，也可以查看照片大图和删除照片。做完该一系列操作后，可提交病害，若病害没有照片会有一次提醒，确认提交后病害会保存到病害列表；若已经在某桩号录入过该类型病害，再次录入会有重复提示。</p>

 <h6><b>③标线缺损、路缘石缺损</b></h6>
 <p style="text-indent:2em;text-align:justify;">这两个页面是比较特殊的病害，所以单独列出。实现了自动检测标线长度和路缘石长度功能。录入缺损长度时，用户确定好开始桩号后点击开始，会提示用户拍摄开始图片，沿着缺损的标线或路缘石向前走直至缺损的终点，点击结束，结束后软件会给出一个推断长度，用户填写标线的系数（0﹤系数≤2.5）后，会计算出一个缺损长度（缺损长度=推断长度X系数），缺损长度不能超过2500m，若超过需用户修改为合适的长度，然后提交，如<a href="#image4">图4</a>。</p>
 <div><img id="image4" src="./_static/4.png" alt="Picture"></div>
 <p style="color: dimgray;text-align: center;">图4  自动采集录入</p>
 <script type="text/javascript">var viewer = new Viewer(document.getElementById('image4'));</script>
 <p style="text-indent:2em;text-align:justify;">若用户觉得系统推断长度不合理，可以自行修改缺损长度。提交时用户可选择提交或提交并继续检测，后者会在提交记录后，以上传记录的结束桩号作为开始桩号开始下一次记录。若选择重新开始，则会清空当前记录，如<a href="#image5">图5</a>。</p>
 <div><img id="image5" src="./_static/5.png" alt="Picture"></div>
 <p style="color: dimgray;text-align: center;">图5  自动采集结束</p>
 <script type="text/javascript">var viewer = new Viewer(document.getElementById('image5'));</script>
 <p style="text-indent:2em;text-align:justify;">页面设有整公里提醒功能，即开始测量标线后若经过一个整公里桩号时，会震动弹框提醒用户结束此次测量，如<a href="#image6">图6</a>。</p>
 <div><img id="image6" src="./_static/6.png" alt="Picture"></div>
 <p style="color: dimgray;text-align: center;">图6  整公里自动采集结束</p>
 <script type="text/javascript">var viewer = new Viewer(document.getElementById('image6'));</script>
 <p style="text-indent:2em;text-align:justify;">若同时考虑页面的整公里校对功能和路线桩号增减的属性对标线缺损整公里弹框的影响，会产生一些比较复杂的情况，在这里做一下说明（现在均没有考虑往回走或者弯道问题）：</p>
 <ul>
 <li>桩号为递增，000≤桩号尾数≤500且标线缺损正在进行，此时整公里校对，不会出现标线缺损弹框；</li>
 <li>桩号为递增，500＜桩号尾数＜999且标线缺损正在进行，此时整公里校对，会出现标线缺损弹框；</li>
 <li>桩号为递减，000＜桩号尾数≤500且标线缺损正在进行，此时整公里校对，会出现标线缺损弹框；</li>
 <li>桩号为递减，500＜桩号尾数＜999且标线缺损正在进行，此时整公里校对，不会出现标线缺损弹框。</li>
 </ul>
 <p style="text-indent:2em;text-align:justify;padding: 0;margin: 0;">若标线和路缘石都在采集中且都经过整公里时，页面会弹出综合提醒，如<a href="#image7">图7</a>。</p>
 <p style="text-indent:2em;text-align:justify;">随后只要这两个页面中存在未提交的整公里记录，左侧导航栏中标线缺损和路缘石缺损都会有一个红色图标进行提醒，直到用户提交完此次记录。</p>
 <div><img id="image7" src="./_static/7.png" alt="Picture"></div>
 <p style="color: dimgray;text-align: center;">图7  整公里自动采集结束</p>
 <script type="text/javascript">var viewer = new Viewer(document.getElementById('image7'));</script>

 <h6><b>④病害列表</b></h6>
 <p style="text-indent:2em;text-align:justify;">该页面主要用于对病害的统计查询，如<a href="#image8">图8</a>。列表中的病害类型为二级病害，用户可查看每条病害的具体信息，同时也可以编辑已提交的病害和删除病害。编辑病害分为编辑录入数据和病害类型两种，删除病害后，用户可通过查询已删除病害，点击病害后的回复按钮进行恢复。查询病害时，用户可输入一个整公里桩号或是普通桩号，软件会查询出所输入桩号上下500米范围内的所有病害。</p>
 <div><img id="image8" src="./_static/8.png" alt="Picture"></div>
 <p style="color: dimgray;text-align: center;">图8  病害列表</p>
 <script type="text/javascript">var viewer = new Viewer(document.getElementById('image8'));</script>

 <h6><b>⑤桩号校对</b></h6>
 <p style="text-indent:2em;text-align:justify;">该页面的功能主要是方便用户实时校对桩号信息，如<a href="#image9">图9</a>。用户可以刷新实时定位桩号（右上角桩号），若定位桩号不准确也可选择页面右侧所提供的备选桩号，选择后点击确定，右上角实时定位桩号也会更新为所选择的桩号。若是备选桩号中也没有合适桩号，用户也可自己手动输入桩号。</p>
 <div><img id="image9" src="./_static/9.png" alt="Picture"></div>
 <p style="color: dimgray;text-align: center;">图9  桩号校对</p>
 <script type="text/javascript">var viewer = new Viewer(document.getElementById('image9'));</script>