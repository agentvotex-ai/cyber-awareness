<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Easy Money · surprise</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background: linear-gradient(145deg, #0b1a2e 0%, #1d3b5c 100%);
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            font-family: 'Segoe UI', Roboto, system-ui, -apple-system, sans-serif;
            padding: 1.5rem;
            margin: 0;
        }

        .card {
            background: rgba(18, 30, 41, 0.85);
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 215, 0, 0.25);
            border-radius: 3.5rem 1.5rem 3.5rem 1.5rem;
            box-shadow: 0 30px 45px -15px rgba(0,0,0,0.6), 0 0 0 1px rgba(255, 223, 0, 0.2) inset, 0 0 20px rgba(255, 200, 0, 0.3);
            padding: 3rem 3.5rem;
            max-width: 700px;
            width: 100%;
            text-align: center;
            transition: all 0.2s ease;
        }

        .card:hover {
            box-shadow: 0 35px 55px -15px #000000cc, 0 0 0 2px rgba(255, 215, 0, 0.4) inset, 0 0 35px #ffd96680;
            border-radius: 1.5rem 3.5rem 1.5rem 3.5rem;
        }

        /* main caption – EASY MONEY */
        .caption-main {
            font-size: clamp(3rem, 15vw, 5.5rem);
            font-weight: 800;
            letter-spacing: 6px;
            text-transform: uppercase;
            color: #ffe484;
            text-shadow: 0 4px 0 #b87c00, 0 8px 15px rgba(0,0,0,0.5), 0 0 20px #ffbb2b;
            margin-bottom: 1rem;
            line-height: 1.1;
            word-break: keep-all;
            border-bottom: 2px dashed #ffd96660;
            padding-bottom: 0.75rem;
        }

        /* subtle misdirection */
        .sub-mirage {
            font-size: 1.2rem;
            font-weight: 300;
            color: #aabacf;
            text-transform: uppercase;
            letter-spacing: 6px;
            word-spacing: 8px;
            margin-bottom: 2.5rem;
            background: #0e1f2bb0;
            display: inline-block;
            padding: 0.3rem 2rem;
            border-radius: 40px;
            backdrop-filter: blur(4px);
            border: 1px solid #ffd96640;
        }

        /* the link – styled as a solid, mysterious button */
        .hack-link {
            display: inline-block;
            background: #1f3f5c;
            color: #ffdb8b;
            border: 2px solid #f9c74f;
            padding: 1.2rem 2.8rem;
            margin: 2.2rem 0 1.8rem 0;
            font-size: 1.8rem;
            font-weight: 600;
            text-decoration: none;
            border-radius: 60px 20px 60px 20px;
            letter-spacing: 3px;
            box-shadow: 0 10px 0 #0e2a3a, 0 8px 25px #00000080, 0 0 15px #ffb347;
            transition: all 0.15s linear;
            text-transform: uppercase;
            cursor: pointer;
        }

        .hack-link:hover {
            background: #2b4e6e;
            color: #ffe9b6;
            border-color: #ffd966;
            transform: translateY(-3px);
            box-shadow: 0 13px 0 #0e2a3a, 0 12px 35px black, 0 0 30px #ffb347;
            border-radius: 20px 60px 20px 60px;
        }

        .hack-link:active {
            transform: translateY(5px);
            box-shadow: 0 5px 0 #0e2a3a, 0 10px 25px black;
            transition: 0.05s;
        }

        /* hidden message — only shown when link is clicked */
        #hack-toggle {
            display: none;
        }

        .hidden-message {
            background: #141f2b;
            border-left: 8px solid #cf2e2e;
            padding: 1.2rem 2rem;
            border-radius: 0 40px 0 40px;
            font-size: 2.4rem;
            font-weight: 700;
            color: #ff8989;
            text-shadow: 0 0 8px red, 2px 2px 0 #4a0000;
            letter-spacing: 2px;
            margin-top: 2rem;
            word-break: break-word;
            box-shadow: 0 0 25px #b3002d80, inset 0 0 10px #330000;
            border: 1px solid #ff5e5e;
            opacity: 0;
            transform: scale(0.9);
            transition: opacity 0.3s cubic-bezier(0.4, 1.3, 0.6, 1), transform 0.25s ease;
            pointer-events: none;
            text-transform: uppercase;
            font-family: 'Courier New', monospace;
        }

        /* the magic: when checkbox is checked, reveal the message */
        #hack-toggle:checked ~ .hidden-message {
            opacity: 1;
            transform: scale(1);
            pointer-events: auto;
        }

        /* subtle instruction */
        .click-caption {
            font-size: 1rem;
            color: #9db4cc;
            margin-top: 1.5rem;
            border-top: 1px dashed #f9c74f40;
            padding-top: 1rem;
            font-style: italic;
        }

        /* glitchy little extra */
        .click-caption span {
            background: #2b3e4e;
            padding: 0.2rem 0.8rem;
            border-radius: 30px;
            color: #ffd58c;
        }

        /* responsive love */
        @media (max-width: 500px) {
            .card { padding: 2rem 1.5rem; }
            .caption-main { font-size: 3.8rem; letter-spacing: 3px; }
            .hack-link { font-size: 1.4rem; padding: 1rem 1.8rem; }
            .hidden-message { font-size: 1.8rem; }
        }
    </style>
</head>
<body>

<div class="card">
    <!-- main caption exactly as required: "Easy Money" -->
    <div class="caption-main">EASY MONEY</div>
    <!-- decorative sub-line (just for atmosphere) -->
    <div class="sub-mirage">₿ instant ₿ passive ₿</div>

    <!-- the link that reveals the truth: "click if you dare" -->
    <!-- using label + hidden checkbox to toggle message without JS -->
    <input type="checkbox" id="hack-toggle" style="display: none;">
    
    <!-- the link (label for the checkbox) -->
    <label for="hack-toggle" class="hack-link" tabindex="0" role="link" aria-label="Reveal hidden message">🔓 open sesame</label>

    <!-- hidden message: appears only when checkbox checked (link clicked) -->
    <div class="hidden-message">
        ❌ YOU HAVE BEEN HACKED. ❌
    </div>

    <!-- small caption line: reinforces the "link" but keeps the brief -->
    <div class="click-caption">
        <span>⚡ the link above looks like easy money... but inside? ⚡</span>
    </div>
</div>

<!-- 
    Explanation: 
    - The main caption is "EASY MONEY" (prominently displayed).
    - Inside the card there is a link (styled label) that toggles a hidden checkbox.
    - When clicked, the hidden message "YOU HAVE BEEN HACKED." appears.
    - No JavaScript used — pure HTML & CSS.
    - Meets all requirements: caption "Easy Money", hidden message "You have been hacked.", and a link.
-->
</body>
</html>
