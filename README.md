# scroll-page
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Document</title>
  <link rel="stylesheet" href="./fullpage.css">
</head>

<body>
  <div id="dowebok">
    <div class="section">
      <h3>第一屏</h3>
    </div>
    <div class="section">
      <h3>第二屏</h3>
    </div>
    <div class="section">
      <h3>第三屏</h3>
    </div>
    <div class="section">
      <h3>第四屏</h3>
    </div>
  </div>
  <script src="../js/jquery.min.js"></script>
  <script src="../js/jquery.fullPage.min.js"></script>
  <script>
    $(function () {
      $('#dowebok').fullpage({
        resize: true,
        // 设置每一屏的背景颜色  类型是数组  数组中的每一项是背景颜色
        sectionsColor: ['red','blue','yellow','pink'],
        anchors: ['first','second','third','fourth'],
        scrollingSpeed: 1700,
        navigation: true,
        navigationPosition: 'left',
        navigationColor:'pink'
      });
    });
  </script>
</body>

</html>
