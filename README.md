<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday Monu</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #fefbd8;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            overflow: hidden;
            background: linear-gradient(135deg, #ff9a8b, #ff6a00);
        }
        .book {
            width: 500px;
            height: 700px;
            background-color: #fff;
            border-radius: 10px;
            box-shadow: 0 0 30px rgba(0, 0, 0, 0.1);
            position: relative;
            overflow: hidden;
            border: 5px solid #ff6a00;
        }
        .page {
            width: 100%;
            height: 100%;
            position: absolute;
            background-color: #fff;
            color: #333;
            padding: 30px;
            box-sizing: border-box;
            font-size: 18px;
            opacity: 0;
            display: none;
            text-align: right;
            line-height: 1.6;
            font-family: 'Courier New', Courier, monospace;
            color: #333;
            background: #fdf6e3;
            transition: opacity 1s ease-in-out;
        }
        .page.active {
            opacity: 1;
            display: block;
        }
        .title {
            font-size: 24px;
            font-weight: bold;
            color: #e74c3c;
            text-align: center;
        }
        .candles {
            font-size: 35px;
            margin-top: 20px;
            text-align: center;
        }
        .bouquet, .cake {
            font-size: 40px;
            margin-top: 20px;
            text-align: center;
        }
        .footer {
            font-size: 18px;
            margin-top: 40px;
            color: #2c3e50;
            font-family: 'Courier New', Courier, monospace; /* Same font as 'dearest monu' */
            text-align: left; /* Align to the left */
            padding-left: 30px;
        }
        button {
            background-color: #e74c3c;
            color: white;
            padding: 10px 20px;
            font-size: 18px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            margin-top: 20px;
        }
        button:hover {
            background-color: #c0392b;
        }
        .navigation-buttons {
            display: flex;
            justify-content: space-between;
            margin-top: 20px;
        }
    </style>
</head>
<body>

<div class="book">
    <!-- First Page - Empty and Cute -->
    <div class="page page1">
        <div class="title">happy birthday monu!</div>
        <div class="candles">🕯️🕯️🕯️</div>
    </div>

    <!-- Second Page - Starts with "Dearest Monu" -->
    <div class="page page2">
        <p><strong>dearest monu,</strong><br><br>
        happy birthdayyyyy broooo! u 15 nowww daamn time movin so fast i still remember when u was jus a kid all goofy and wild and soft n now u here growin up and all that shit and idk why but today i just couldn’t keep quiet i had to say somethin cos this day it dont feel like jus another day to me bro this day special cos its the day u came into this world and i knw that sound dramatic but its true cos if u wasn’t born i wouldn’t have met u and bro that thought itself make my chest feel heavy cos meetin u really changed me fr like in ways i don’t even have full words for yet i still remember the first time we talked how u made me feel safe how u looked at me like u actually saw me like u understood me without me even sayin much.</p>
    </div>

    <!-- Third Page -->
    <div class="page page3">
        <p>and even now after everything after we not together no more i still feel that same warmth when i think about u and that shit don’t just go away bro no matter how much i try to act cool or like i moved on or whatever deep down i still love u bro i do and i’m not sayin this to make u uncomfortable or to mess with ur peace or nothin i just needed u to know that my heart still carryin a piece of u always and yeah maybe we not where we used to be maybe we jus got memories now but those memories real and they soft and they mean a lot to me and bro u was never jus someone i dated u was someone i loved for real someone i still love jus in a quieter way now.</p>
    </div>

    <!-- Fourth Page -->
    <div class="page page4">
        <p>and i miss it sometimes not gonna lie i miss u sometimes more than i know how to say like i miss ur voice and the way u used to text me random dumb shit or how u always made me feel okay even on my worst days and maybe u dont feel the same anymore maybe u moved on and thats okay too cos i aint sayin this to bring anything back i’m jus sayin it cos its real and i wanna be honest wit my heart for once and i hope u having a good day today i hope u smiling and feelin love all around u cos u deserve that u really do bro u always had a heart too big too soft too good for this world and i hope the people around u now see that and treat it right.</p>
    </div>

    <!-- Fifth Page -->
    <div class="page page5">
        <p>whoever come next in ur life i jus hope she sees the same things i saw in u i hope she knows how lucky she is cos u love different bro u love deep and soft and loud in ur own way and if she don’t appreciate that then she don’t deserve u at all and even tho we not together no more i’m still here silently wishin u all the good shit in life still rooting for u from far still loving u in my own quiet way cos that love never left it just changed and even if we never talk again even if we jus strangers with memories now i’ll still be carryin u with me in little ways like in songs or places or moments that remind me of us.</p>
    </div>

    <!-- Sixth Page -->
    <div class="page page6">
        <p>and sometimes that make me sad but mostly it make me grateful that i even got to love u at all even if it was for a little while so happy birthday again bro u still mean so much to me and u always will.</p>
        <div class="footer">yours lovingly, divyanshi</div>
    </div>
</div>

<div class="navigation-buttons">
    <button onclick="prevPage()">previous page</button>
    <button onclick="nextPage()">next page</button>
</div>

<script>
    let currentPage = 1;
    const totalPages = 6;

    function nextPage() {
        if (currentPage < totalPages) {
            document.querySelector(`.page${currentPage}`).classList.remove('active');
            currentPage++;
            document.querySelector(`.page${currentPage}`).classList.add('active');
        }
    }

    function prevPage() {
        if (currentPage > 1) {
            document.querySelector(`.page${currentPage}`).classList.remove('active');
            currentPage--;
            document.querySelector(`.page${currentPage}`).classList.add('active');
        }
    }

    // Initially show the first page
    document.querySelector(`.page${currentPage}`).classList.add('active');
</script>

</body>
</html>
