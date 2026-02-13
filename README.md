# School-website
School system
<!DOCTYPE html>
<html lang="ar">
<head>
  <meta charset="UTF-8">
  <title>التواصل عبر واتساب - مدرسة يزيد بن حاتم الأزدي</title>
  <link rel="stylesheet" href="style.css">
  <script>
    function sendWhatsApp() {
      var name = document.getElementById("name").value;
      var email = document.getElementById("email").value;
      var message = document.getElementById("message").value;

      // رقم واتساب الرسمي للمدرسة (ضع الرقم هنا بصيغة دولية)
      var phone = "96891234567"; // مثال: عمان (+968)

      var text = "الاسم: " + name + "%0aالبريد: " + email + "%0aالرسالة: " + message;
      var url = "https://wa.me/" + phone + "?text=" + text;

      window.open(url, "_blank");
    }
  </script>
</head>
<body>
  <header>
    <h1>التواصل عبر واتساب</h1>
  </header>

  <nav>
    <a href="index.html">الرئيسية</a>
    <a href="news.html">الأخبار</a>
    <a href="schedules.html">الجداول</a>
    <a href="contact.html">التواصل</a>
  </nav>

  <main>
    <h2>أرسل لنا رسالة عبر واتساب</h2>
    <form onsubmit="sendWhatsApp(); return false;">
      <label for="name">الاسم:</label><br>
      <input type="text" id="name" name="name" required><br><br>

      <label for="email">البريد الإلكتروني:</label><br>
      <input type="email" id="email" name="email" required><br><br>

      <label for="message">الرسالة:</label><br>
      <textarea id="message" name="message" rows="5" required></textarea><br><br>

      <button type="submit">إرسال عبر واتساب</button>
    </form>
  </main>

  <footer>
    &copy; 2026 مدرسة يزيد بن حاتم الأزدي - جميع الحقوق محفوظة
  </footer>
</body>
</html>
