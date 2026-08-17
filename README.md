<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>لسه بتحبني؟ ❤️</title>

<style>
@import url('https://fonts.googleapis.com/css2?family=Amiri:wght@400;700&family=Cairo:wght@400;600;700&display=swap');

* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

html {
    scroll-behavior: smooth;
}

body {
    min-height: 100vh;
    background:
        radial-gradient(circle at 20% 20%, rgba(255,120,170,.22), transparent 30%),
        radial-gradient(circle at 80% 80%, rgba(170,80,190,.18), transparent 35%),
        linear-gradient(135deg, #120712, #351326, #16091b);

    color: white;
    font-family: "Amiri", serif;
    overflow-x: hidden;
}

/* =========================
   القلوب المتحركة
========================= */

.heart {
    position: fixed;
    bottom: -50px;
    z-index: 0;
    color: rgba(255,180,205,.35);
    pointer-events: none;
    animation: floatHeart linear infinite;
}

@keyframes floatHeart {

    0% {
        transform: translateY(0) rotate(0deg);
        opacity: 0;
    }

    15% {
        opacity: 1;
    }

    100% {
        transform: translateY(-115vh) rotate(360deg);
        opacity: 0;
    }
}

/* =========================
   شاشة البداية
========================= */

.start-screen {

    min-height: 100vh;

    display: flex;
    flex-direction: column;

    align-items: center;
    justify-content: center;

    text-align: center;

    padding: 25px;

    position: relative;
    z-index: 2;
}

.start-small {

    color: #eab3c8;

    font-family: Cairo, sans-serif;

    font-size: 14px;

    letter-spacing: 2px;

    margin-bottom: 15px;
}

.start-screen h1 {

    font-size: clamp(45px, 11vw, 85px);

    color: #ffd9e5;

    text-shadow:
        0 0 15px rgba(255,150,190,.5),
        0 0 40px rgba(255,100,160,.25);

    animation: heartbeat 2s infinite;
}

@keyframes heartbeat {

    0%,100% {
        transform: scale(1);
    }

    50% {
        transform: scale(1.05);
    }
}

.question {

    margin-top: 10px;

    font-size: clamp(20px,4vw,28px);

    color: #f5d8e2;
}

.buttons {

    position: relative;

    width: 100%;

    max-width: 500px;

    height: 130px;

    margin-top: 35px;

    display: flex;

    justify-content: center;

    align-items: center;

    gap: 20px;
}

.choice {

    border: none;

    padding: 14px 35px;

    border-radius: 50px;

    font-family: Cairo, sans-serif;

    font-size: 16px;

    cursor: pointer;

    transition: .3s;
}

.yes {

    background: linear-gradient(135deg,#ed91ae,#b9557b);

    color: white;

    box-shadow:
        0 10px 30px rgba(220,100,145,.35);
}

.yes:hover {

    transform: scale(1.08);
}

.no {

    background: rgba(255,255,255,.1);

    color: #f0dce3;

    border: 1px solid rgba(255,255,255,.2);

    position: relative;
}

.hint {

    margin-top: 10px;

    color: rgba(255,255,255,.55);

    font-family: Cairo,sans-serif;

    font-size: 12px;
}

/* =========================
   كل الأقسام
========================= */

#story {

    display: none;

    position: relative;

    z-index: 2;

    animation: appear 1.2s ease;
}

.section {

    min-height: 100vh;

    width: min(900px,92%);

    margin: auto;

    padding: 70px 0;

    display: flex;

    flex-direction: column;

    justify-content: center;

    align-items: center;

    text-align: center;
}

/* =========================
   الصور
========================= */

.photo-box {

    width: min(650px,95%);

    height: 480px;

    border-radius: 30px;

    overflow: hidden;

    background: rgba(255,255,255,.08);

    border: 1px solid rgba(255,255,255,.18);

    box-shadow:
        0 30px 70px rgba(0,0,0,.45);

    animation: photoAppear 1.5s ease;
}

<img src="photo1.jpg">

    width: 100%;

    height: 100%;

    object-fit: cover;
}

.photo-caption {

    margin-top: 25px;

    font-size: 30px;

    color: #ffd5e1;

    text-shadow:
        0 0 15px rgba(255,150,190,.3);
}

@keyframes photoAppear {

    from {

        opacity: 0;

        transform:
            scale(.9)
            translateY(30px);
    }

    to {

        opacity: 1;

        transform:
            scale(1)
            translateY(0);
    }
}

/* =========================
   الشاشة السوداء
========================= */

.black-screen {

    min-height: 100vh;

    background: #000;

    display: flex;

    flex-direction: column;

    justify-content: center;

    align-items: center;

    padding: 30px;

    text-align: center;
}

.black-screen .sad-text {

    font-size: clamp(25px,5vw,42px);

    line-height: 1.8;

    color: #f2f2f2;

    animation: fadeText 3s ease;
}

.black-screen .small-text {

    margin-top: 25px;

    color: #777;

    font-size: 18px;
}

@keyframes fadeText {

    from {
        opacity: 0;
    }

    to {
        opacity: 1;
    }
}

/* =========================
   الرسالة
========================= */

.letter-section {

    min-height: auto;

    padding-top: 100px;

    padding-bottom: 100px;
}

.card {

    background: rgba(255,255,255,.075);

    border: 1px solid rgba(255,255,255,.15);

    border-radius: 30px;

    padding: clamp(25px,6vw,55px);

    backdrop-filter: blur(14px);

    box-shadow:
        0 25px 70px rgba(0,0,0,.35);
}

.letter-title {

    font-size: 42px;

    color: #ffd3df;

    margin-bottom: 35px;
}

.message {

    font-size: clamp(20px,3vw,27px);

    line-height: 2.2;

    color: #fff4f7;
}

.message span {

    color: #ffb8cc;
}

.divider {

    width: 100px;

    height: 2px;

    background: #e9a6bc;

    margin: 40px auto;

    box-shadow:
        0 0 15px #e9a6bc;
}

/* =========================
   الموسيقى
========================= */

.music-section {

    min-height: 70vh;
}

.music-title {

    font-size: 35px;

    color: #ffd3df;

    margin-bottom: 20px;
}

.music-text {

    color: #d7b7c4;

    font-size: 18px;

    margin-bottom: 30px;
}

.music-button {

    border: none;

    padding: 16px 32px;

    border-radius: 50px;

    background:
        linear-gradient(135deg,#d987a4,#a95b7b);

    color: white;

    font-family: Cairo,sans-serif;

    font-size: 15px;

    cursor: pointer;

    box-shadow:
        0 10px 30px rgba(190,100,140,.3);

    transition: .3s;
}

.music-button:hover {

    transform: scale(1.05);
}

/* =========================
   النهاية
========================= */

.final-section {

    min-height: 80vh;
}

.final-heart {

    font-size: 65px;

    margin-bottom: 25px;

    animation: heartbeat 2s infinite;
}

.final-text {

    font-size: clamp(27px,5vw,45px);

    line-height: 1.8;

    color: #ffd8e3;
}

.final-small {

    margin-top: 30px;

    color: #d3aebb;

    font-size: 19px;
}

@keyframes appear {

    from {

        opacity: 0;

        transform: translateY(35px);
    }

    to {

        opacity: 1;

        transform: translateY(0);
    }
}

/* =========================
   الموبايل
========================= */

@media(max-width:650px) {

    .photo-box {

        height: 400px;
    }

    .message {

        line-height: 2;
    }

    .section {

        padding: 50px 0;
    }
}
</style>
</head>


<body>


<!-- =========================
     القلوب
========================= -->

<div class="heart" style="left:5%;font-size:25px;animation-duration:9s;">♥</div>
<div class="heart" style="left:15%;font-size:18px;animation-duration:12s;animation-delay:2s;">♡</div>
<div class="heart" style="left:28%;font-size:30px;animation-duration:10s;animation-delay:4s;">♥</div>
<div class="heart" style="left:42%;font-size:20px;animation-duration:13s;animation-delay:1s;">♡</div>
<div class="heart" style="left:57%;font-size:28px;animation-duration:9s;animation-delay:5s;">♥</div>
<div class="heart" style="left:70%;font-size:19px;animation-duration:11s;animation-delay:3s;">♡</div>
<div class="heart" style="left:84%;font-size:30px;animation-duration:10s;animation-delay:6s;">♥</div>
<div class="heart" style="left:94%;font-size:18px;animation-duration:12s;animation-delay:1s;">♡</div>


<!-- =========================
     البداية
========================= -->

<section class="start-screen" id="start">

    <div class="start-small">
        قبل ما تقرأ أي حاجة...
    </div>

    <h1>
        لسه بتحبني؟!
    </h1>

    <div class="question">
        ولا خلاص مليش غلاوه عندك؟
    </div>

    <div class="buttons">

        <button
            class="choice yes"
            onclick="showStory()">

            أيوه

        </button>


        <button
            class="choice no"
            id="noButton"
            onmouseover="runAway()"
            ontouchstart="runAway()">

            لا

        </button>

    </div>

    <div class="hint">
        فكر كويس قبل ما تختار 😂❤️
    </div>

</section>


<!-- =========================
     القصة
========================= -->

<div id="story">


<!-- =========================
     الصورة الأولى
========================= -->

<section class="section">

    <div class="photo-box">

        <!--
        الصورة الأولى:
        photo1.jpg
        -->

        <img
            src="photo1.jpg"
            alt="مرة وإحنا مع بعض">

    </div>

    <div class="photo-caption">

        مرّة وإحنا مع بعض 🤍

    </div>

</section>


<!-- =========================
     الصورة الثانية
========================= -->

<section class="section">

    <div class="photo-box">

        <!--
        الصورة الثانية:
        photo2.jpg
        -->

        <img
            src="photo2.jpg"
            alt="مرة وإحنا مبسوطين">

    </div>

    <div class="photo-caption">

        ومرّة وإحنا مبسوطين ❤️

    </div>

</section>


<!-- =========================
     الشاشة السوداء
========================= -->

<section class="black-screen">

    <div class="sad-text">

        مفيش صورة وإحنا زعلانين...

        <br>

        لأن حبيبي مش بيحب يزعل مني

    </div>

    <div class="small-text">

        وانا والله مش بحب أزعلك ولو زعلتك ف غصب عني وحقك علي عيني ينورعيني❤️‍🩹

    </div>

</section>


<!-- =========================
     الرسالة
========================= -->

<section class="section letter-section">

<div class="card">

    <div class="letter-title">

        خليك معايا❤️‍🩹

    </div>


    <div class="message">

        أنتَ تعلمُ كم يكونُ البُعدُ قاسيًا،
        فكيفَ يكونُ حينَ يكونُ المرءُ هو مَن صنعَ المسافةَ بيديه؟

        <br><br>

        أعلمُ أنّ في قلبِكَ من العتابِ ما يكفي،
        وأعلمُ أنّ خطئي أثقلَ بيننا المسافة،
        لكنّك لا تعلمُ كيفَ يمضي الوقتُ عليَّ منذ ابتعدتَ.

        <br><br>

        أشتاقُ إليكَ،
        ثمّ يردّني ندمي،
        فأصمتُ…

        <br><br>

        وأظلُّ بينَ رغبةٍ عارمةٍ في أن أقتربَ منك،
        وخوفٍ من أن يكونَ اقترابي في غيرِ موضعِه.

        <br><br>

        ما أقسى أن يشتاقَ المرءُ إلى مَن يحبُّ،
        <span>وأنت كل ما أحب.</span>

        <br><br>

        ليتَكَ تعلمُ أنّني لا أفتقدُ حضورَكَ فحسب،
        بل أفتقدُ طمأنينتي التي كانت تسكنُ بقربِكَ،
        وأفتقدُ ذلك الشعورَ الذي كان يُخبرني
        أنّ لي في هذا العالمِ موضعًا آمنًا،

        <br>

        <span>هو أنت.</span>

        <div class="divider"></div>

        وإن كانَ لي أن أقولَ شيئًا،
        فإنّي أقولُ:

        <br>

        <span>سامحني.</span>

        <br><br>

        فواللهِ ما يؤلمني شيءٌ كما يؤلمني
        أن أكونَ سببًا في حزنِ قلبٍ
        كان كلُّ ما يريده أن يكونَ سعيدًا معي.

    </div>

</div>

</section>


<!-- =========================
     الموسيقى
========================= -->

<section class="section music-section">

    <div class="music-title">

        يمكن الأغنية تقول اللي معرفتش أقوله 🎵

    </div>

    <div class="music-text">

        اسمعها للآخر 🤍

    </div>


    <button
        class="music-button"
        onclick="toggleMusic()">

        🎵 تشغيل الأغنية

    </button>


    <!--
    ضعي أغنية حماقي هنا
    واسم الملف يكون:
    song.mp3
    -->

    <audio id="music">

        <source
            src="song.mp3"
            type="audio/mpeg">

    </audio>

</section>


<!-- =========================
     النهاية
========================= -->

<section class="section final-section">

    <div class="final-heart">
        ❤️
    </div>

    <div class="final-text">

        ينفع نرجع زي الأول وأحسن؟

        <br>

        وأوعدك، عمري ما هزعلك تاني.

        <br>

        خلّينا نبدأ من جديد،
        بس المرة دي وإحنا متمسكين ببعض أكتر. 🤍

    </div>

    <div class="final-small">

        لأنّي لسه شايفة إن أجمل مكان ليا... هو جنبك.

    </div>

</section>


</div>


<script>

/* =========================
   زر لا يهرب 😂
========================= */

const noButton =
    document.getElementById("noButton");

function runAway() {

    const maxX =
        window.innerWidth -
        noButton.offsetWidth -
        20;

    const maxY =
        window.innerHeight -
        noButton.offsetHeight -
        20;

    const x =
        Math.max(10, Math.random() * maxX);

    const y =
        Math.max(10, Math.random() * maxY);

    noButton.style.position = "fixed";

    noButton.style.left =
        x + "px";

    noButton.style.top =
        y + "px";

    noButton.style.zIndex = "9999";
}


/* =========================
   فتح القصة
========================= */

function showStory() {

    document.getElementById("start").style.display =
        "none";

    document.getElementById("story").style.display =
        "block";

    window.scrollTo({
        top: 0,
        behavior: "smooth"
    });
}


/* =========================
   الموسيقى
========================= */

function toggleMusic() {

    const music =
        document.getElementById("music");

    const button =
        document.querySelector(".music-button");


    if (music.paused) {

        music.play();

        button.innerHTML =
            "⏸️ إيقاف الأغنية";

    } else {

        music.pause();

        button.innerHTML =
            "🎵 تشغيل الأغنية";
    }
}

</script>

</body>
</html>
