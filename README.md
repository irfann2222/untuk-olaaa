<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>olaaa sayang</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f8e1e1; /* Soft pink background */
            font-family: 'Georgia', serif; /* Elegant font */
        }

        .envelope {
            width: 800px;
            height: 400px;
            background: #fff;
            border: 5px solid #ff6f61; /* Soft coral border */
            border-radius: 15px;
            position: relative;
            cursor: pointer;
            transition: box-shadow 0.3s, transform 0.3s;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
            overflow: hidden; /* Hide overflow for animations */
        }

        .envelope:hover {
            transform: scale(1.05); /* Slightly enlarge on hover */
        }

        .stamp {
            position: absolute;
            top: 190px;
            left: 45%;
            width: 60px;
            height: 60px;
            background: #ffcccb; /* Light pink stamp */
            border: 3px solid #ff6f61; /* Coral border */
            border-radius: 5px;
            box-shadow: 0 2px 5px rgba(119, 76, 76, 0.2);
            text-align: center;
            line-height: 60px;
            font-weight: bold;
            font-size: 24px;
            z-index: 1;
        }

        .touch-text {
            position: absolute;
            top: 35%;
            left: 50%;
            transform: translate(-50%, -50%);
            font-size: 30px;
            color: #9d3a31; /* Coral color */
            z-index: 1;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
            display: block;
            animation: pulse 1.5s infinite; /* Pulsing animation */
        }

        @keyframes pulse {
            0%, 100% {
                transform: translate(-50%, -50%) scale(1);
            }
            50% {
                transform: translate(-50%, -50%) scale(1.1);
            }
        }

        .letter {
            display: none; /* Initially hidden */
            padding: 20px;
            background: #fff;
            border: 2px solid #ff6f61; /* Coral border */
            border-radius: 5px;
            position: absolute;
            top: 20px;
            left: 20px;
            right: 20px;
            bottom: 20px;
            z-index: 2;
            overflow-y: auto;
            font-size: 20px;
            color: #333;
        }

        .envelope.open {
            box-shadow: 0 0 15px rgba(0, 0, 0, 0.3);
        }

        .envelope.open .letter {
            display: block; /* Show letter when open */
        }

        .envelope.open .touch-text {
            display: none; /* Hide when the envelope is open */
        }
    </style>
</head>
<body>

<div class="envelope" onclick="toggleEnvelope(this)">
    <div class="stamp">❤️</div> <!-- Romantic stamp -->
    <div class="touch-text">touch this heart olaaa! </div> <!-- Romantic text -->
    <div class="letter">
        my dearest,<br><br>
        haii olaa!! aku mau balas surat lucu yg uda kamu buat untuk aku:))<br>
        you know, kamu itu best experience aku tahun ini, kaya lucu aja w main tele trus like ur profile n then 
        gatau tiba tiba kita di citra ketemu ahaha w masi ingat mata kamu lucu bgtt pas pakai cakil, mana awalnya lu kira w tukang ojek.<br><br>
        tapi yang keingat bener itu our secdate. lu canti parah kemarin itu, you just like kind to me
        dan gatau kenapa hari itu waktu bener bener kerasa bentar aaaarhg. intinya tiap ketemu kamuuu aku seneng bgt butt...<br>
        aku mau minta maaf krn tiap ketemu selalu kamu yg cari topik, maaf ya aku sering diem kalau di samping kamu, gatau juga kenapa gitu,
        topiknya uda disiapin tapi kalau uda liat mata lu, gatau kemana topikny pergi.<br><br>
        aku senang bisa dengar semua cerita dari kamu, kalau kamu butuh teman buat ngobrol, just talk to me yaa, 
        u need to remember you re enough, even more than enough, kalau cape take a rest okkaii jangan maksain cz no one is perfect tetap jadi olaa yang aku kenal
        terahkhir i wanna say, WE LL NEVER LOSE EACH OTHER !
        lu orang baik yg harus ada di akhir hidup w, w seneng main sama lu jadi next gw jemput pulang skull yaaaa!<br>
        thank u for all the love u have given to me 🤍<br><br>
        loovvee youu<br>
        XOXO
    </div>
</div>

<script>
    function toggleEnvelope(el) {
        el.classList.toggle('open');
    }
</script>

</body>
</html>
