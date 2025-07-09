<!DOCTYPE html>
<html lang="zh-Hant">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Meta Pixel 測試頁面</title>

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
    fbq('init', '1680984415874629'); 
    fbq('track', 'PageView');
  </script>
  <noscript>
    <img height="1" width="1" style="display:none"
      src="https://www.facebook.com/tr?id=1680984415874629&ev=PageView&noscript=1"/>
  </noscript>
  <!-- End Meta Pixel Code -->

  <style>
    body {
      font-family: "Helvetica Neue", sans-serif;
      text-align: center;
      padding: 50px;
    }
    button {
      font-size: 18px;
      padding: 12px 24px;
      margin: 12px;
      border: none;
      background-color: #4267B2;
      color: white;
      border-radius: 8px;
      cursor: pointer;
    }
    button:hover {
      background-color: #365899;
    }
  </style>
</head>
<body>

  <h1>👋 歡迎來到 Pixel 測試站！</h1>
  <p>這是一個用來測試 Facebook Pixel 事件的簡單頁面。</p>

  <button onclick="fbq('track', 'AddToCart'); alert('🛒 已觸發加購事件')">
    🛒 模擬加購
  </button>

  <button onclick="fbq('track', 'Purchase', {value: 1998, currency: 'TWD'}); alert('💰 已觸發購買事件')">
    💰 模擬購買
  </button>
  
  <button onclick="fbq('trackCustom', 'ViewFAQ'); alert('📖 已触发 ViewFAQ 自定义事件')">
  ❓ 查看常見問題
</button>
 fbq('trackCustom', 'ViewFAQ', {
  section: 'shipping_policy'
})


</body>
</html>
