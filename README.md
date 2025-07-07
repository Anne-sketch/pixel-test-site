<!DOCTYPE html>
<html>
<head>
  <title>Pixel 测试页面</title>
  <!-- Meta Pixel Code -->
  <script>
    !function(f,b,e,v,n,t,s)
    {if(f.fbq)return;n=f.fbq=function(){n.callMethod?
    n.callMethod.apply(n,arguments):n.queue.push(arguments)};
    if(!f._fbq)f._fbq=n;n.push=n;n.loaded=!0;n.version='2.0';
    n.queue=[];t=b.createElement(e);t.async=!0;
    t.src=v;s=b.getElementsByTagName(e)[0];
    s.parentNode.insertBefore(t,s)}(window, document,'script',
    'https://connect.facebook.net/en_US/fbevents.js');
    fbq('init', '你的 Pixel ID 替换这里'); 
    fbq('track', 'PageView');
  </script>
  <noscript>
    <img height="1" width="1" style="display:none"
      src="https://www.facebook.com/tr?id= 1680984415874629&ev=PageView&noscript=1"/>
  </noscript>
  <!-- End Meta Pixel Code -->
</head>
<body>
  <h1>🎯 Meta Pixel 测试页面</h1>
  <p>欢迎来到我的 Pixel 测试页面。点击下方按钮进行事件测试：</p>

  <button onclick="fbq('track', 'AddToCart'); alert('🛒 加购事件已触发')">
    🛒 模拟加购
  </button>

  <br><br>

  <button onclick="fbq('track', 'Purchase', {value: 1998, currency: 'TWD'}); alert('💰 购买事件已触发')">
    💰 模拟购买
  </button>
</body>
</html>
