<!DOCTYPE html>
<html lang="fa">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>آزمون تیزهوشانی 🎓</title>
  <style>
    body {
      font-family: sans-serif;
      direction: rtl;
      background-color: #eef2ff;
      text-align: center;
      padding: 30px;
    }
    .question-box {
      background: #fff;
      padding: 25px;
      border-radius: 15px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      max-width: 450px;
      margin: 40px auto;
    }
    .option {
      background: #dbeafe;
      padding: 12px;
      border-radius: 10px;
      margin: 10px 0;
      cursor: pointer;
      transition: background 0.3s;
    }
    .option:hover { background: #bfdbfe; }
    .correct { background: #86efac !important; }
    .wrong { background: #fca5a5 !important; }
    .result { margin-top: 15px; font-weight: bold; }
    .nextBtn {
      display: none;
      margin-top: 15px;
      background-color: #3b82f6;
      color: white;
      border: none;
      padding: 10px 20px;
      border-radius: 10px;
      cursor: pointer;
    }
  </style>
</head>
<body>

  <!-- سوال ۱ (آسان) -->
  <div class="question-box" id="q1">
    <h3>سؤال ۱:</h3>
    <p>کدام کاغذ بهتر است؟</p>
    <div class="option" onclick="checkAnswer(this, false)">کاغذ سفید</div>
    <div class="option" onclick="checkAnswer(this, true)">کاغذ بازیافتی</div>
    <div class="option" onclick="checkAnswer(this, false)">کاغذ رنگی</div>
    <div class="option" onclick="checkAnswer(this, false)">کاغذ نازک</div>
    <div class="result"></div>
    <button class="nextBtn" onclick="showQuestion(2)">سؤال بعد ➡️</button>
  </div>

  <!-- سوال ۲ (آسان) -->
  <div class="question-box" id="q2" style="display:none;">
    <h3>سؤال ۲:</h3>
    <p>کدام کار به حفظ محیط‌زیست کمک می‌کند؟</p>
    <div class="option" onclick="checkAnswer(this, false)">ریختن زباله در خیابان</div>
    <div class="option" onclick="checkAnswer(this, true)">خاموش کردن چراغ‌های اضافی</div>
    <div class="option" onclick="checkAnswer(this, false)">بریدن درختان</div>
    <div class="option" onclick="checkAnswer(this, false)">مصرف زیاد آب</div>
    <div class="result"></div>
    <button class="nextBtn" onclick="showQuestion(3)">سؤال بعد ➡️</button>
  </div>

  <!-- سوال ۳ (آسان) -->
  <div class="question-box" id="q3" style="display:none;">
    <h3>سؤال ۳:</h3>
    <p>برای صرفه‌جویی در آب چه باید کرد؟</p>
    <div class="option" onclick="checkAnswer(this, false)">باز گذاشتن شیر آب هنگام مسواک زدن</div>
    <div class="option" onclick="checkAnswer(this, false)">شستن ماشین با شلنگ</div>
    <div class="option" onclick="checkAnswer(this, true)">استفاده از آب کمتر هنگام شستن ظرف‌ها</div>
    <div class="option" onclick="checkAnswer(this, false)">باز گذاشتن آب برای خنک شدن</div>
    <div class="result"></div>
    <button class="nextBtn" onclick="showQuestion(4)">مرحله بعد ➡️</button>
  </div>

  <!-- سوال ۴ (متوسط) -->
  <div class="question-box" id="q4" style="display:none;">
    <h3>سؤال ۴:</h3>
    <p>اگر ۳ گربه در ۳ دقیقه ۳ موش بگیرند، ۶ گربه در ۶ دقیقه چند موش می‌گیرند؟</p>
    <div class="option" onclick="checkAnswer(this, false)">۳ موش</div>
    <div class="option" onclick="checkAnswer(this, true)">۶ موش</div>
    <div class="option" onclick="checkAnswer(this, false)">۹ موش</div>
    <div class="option" onclick="checkAnswer(this, false)">۱۲ موش</div>
    <div class="result"></div>
    <button class="nextBtn" onclick="showQuestion(5)">سؤال بعد ➡️</button>
  </div>

  <!-- سوال ۵ (متوسط) -->
  <div class="question-box" id="q5" style="display:none;">
    <h3>سؤال ۵:</h3>
    <p>در یک خانواده ۲ پدر و ۲ پسر هستند ولی فقط ۳ نفرند. چطور ممکن است؟</p>
    <div class="option" onclick="checkAnswer(this, true)">یکی از پدرها، پدر و پسر هم‌زمان است</div>
    <div class="option" onclick="checkAnswer(this, false)">یکی از آن‌ها دوقلو است</div>
    <div class="option" onclick="checkAnswer(this, false)">یکی از آن‌ها ناپدری است</div>
    <div class="option" onclick="checkAnswer(this, false)">غلط نوشته شده</div>
    <div class="result"></div>
    <button class="nextBtn" onclick="showQuestion(6)">سؤال بعد ➡️</button>
  </div>

  <!-- سوال ۶ (متوسط) -->
  <div class="question-box" id="q6" style="display:none;">
    <h3>سؤال ۶:</h3>
    <p>ساعت ۴:۳۰ است. زاویه بین عقربه ساعت و دقیقه چند درجه است؟</p>
    <div class="option" onclick="checkAnswer(this, false)">۳۰ درجه</div>
    <div class="option" onclick="checkAnswer(this, true)">۴۵ درجه</div>
    <div class="option" onclick="checkAnswer(this, false)">۶۰ درجه</div>
    <div class="option" onclick="checkAnswer(this, false)">۹۰ درجه</div>
    <div class="result"></div>
    <button class="nextBtn" onclick="finishQuiz()">پایان آزمون ✅</button>
  </div>

  <h2 id="finalMessage" style="display:none; color:#10b981;">🎉 آزمون تموم شد! آفرین! 🌟</h2>

  <script>
    function checkAnswer(el, correct) {
      const parent = el.parentElement;
      const options = parent.querySelectorAll('.option');
      options.forEach(o => o.style.pointerEvents = 'none');

      if (correct) {
        el.classList.add('correct');
        parent.querySelector('.result').textContent = "✅ آفرین! پاسخ درسته.";
        parent.querySelector('.nextBtn').style.display = 'inline-block';
      } else {
        el.classList.add('wrong');
        parent.querySelector('.result').textContent = "❌ اشتباهه! دوباره تلاش کن.";
      }
    }

    function showQuestion(num) {
      document.querySelectorAll('.question-box').forEach(q => q.style.display = 'none');
      document.getElementById('q' + num).style.display = 'block';
    }

    function finishQuiz() {
      document.querySelectorAll('.question-box').forEach(q => q.style.display = 'none');
      document.getElementById('finalMessage').style.display = 'block';
    }
  </script>

</body>
</html>
