<!-- 修正版 index.html，標準事件用 track，自訂事件用 trackCustom -->
<!DOCTYPE html>
<html lang="zh-Hant">
<head>
<!-- Google Tag Manager -->
<script>(function(w,d,s,l,i){w[l]=w[l]||[];w[l].push({'gtm.start':
new Date().getTime(),event:'gtm.js'});var f=d.getElementsByTagName(s)[0],
j=d.createElement(s),dl=l!='dataLayer'?'&l='+l:'';j.async=true;j.src=
'https://www.googletagmanager.com/gtm.js?id='+i+dl;f.parentNode.insertBefore(j,f);
})(window,document,'script','dataLayer','GTM-NTJB2KVD');</script>
<!-- End Google Tag Manager -->  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
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
<!-- Google Tag Manager (noscript) -->
<noscript><iframe src="https://www.googletagmanager.com/ns.html?id=GTM-NTJB2KVD"
height="0" width="0" style="display:none;visibility:hidden"></iframe></noscript>
<!-- End Google Tag Manager (noscript) -->
  <h1>👋 歡迎來到 Pixel 測試站！</h1>
  <p>這是一個用來測試 Facebook Pixel 事件的進階頁面。</p>

  <!-- ✅ 標準事件 -->
 <button onclick="fbq('track', 'AddToCart'); alert('🛒 已觸發加購事件')">
  🛒 模擬加購
</button>

    🛒 模擬加購
  </button>

  <button onclick="fbq('track', 'Purchase', {value: 1998, currency: 'TWD'}); alert('💰 已觸發購買事件')">
    💰 模擬購買
  </button>

  <!-- ✅ 自訂事件 -->
  <button onclick="fbq('trackCustom', 'ViewFAQ', {section: 'shipping_policy'}); alert('📖 已觸發：配送政策')">
    ❓ 查看常見問題（配送政策）
  </button>

  <button onclick="fbq('trackCustom', 'ViewFAQ', {section: 'return_policy'}); alert('📖 已觸發：退貨政策')">
    🔁 查看常見問題（退貨政策）
  </button>

  <button onclick="fbq('trackCustom', 'ViewFAQ', {section: 'payment_methods'}); alert('📖 已觸發：付款方式')">
    💳 查看常見問題（付款方式）
  </button>

</body>
</html>
