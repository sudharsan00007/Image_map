# Ex04 Places Around Me
# Date:
# AIM
To develop a website to display details about the places around my house.

# DESIGN STEPS
## STEP 1
Create a Django admin interface.

## STEP 2
Download your city map from Google.

## STEP 3
Using <map> tag name the map.

## STEP 4
Create clickable regions in the image using <area> tag.

## STEP 5
Write HTML programs for all the regions identified.

## STEP 6
Execute the programs and publish them.

# CODE
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Image Map - Neon Style</title>
    <style>
        /* Neon gradient background */
        body {
            margin: 0;
            padding: 0;
            background: linear-gradient(135deg, #ff0080, #ff8000, #00ffcc, #0080ff);
            background-size: 400% 400%;
            animation: gradientBG 15s ease infinite;
            color: #fff;
            font-family: Arial, sans-serif;
        }

        /* Animation for background */
        @keyframes gradientBG {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        /* Center image */
        img {
            display: block;
            margin: 20px auto;
            border: 5px solid rgba(255, 255, 255, 0.5);
            box-shadow: 0 0 20px rgba(255, 255, 255, 0.7);
        }

        /* Glowing hover effect on map areas */
        area {
            outline: none;
        }
        area:hover {
            filter: brightness(1.5);
        }

        /* Style for character sections */
        div {
            margin: 20px auto;
            padding: 20px;
            max-width: 800px;
            border: 2px solid rgba(255, 255, 255, 0.7);
            border-radius: 10px;
            box-shadow: 0 0 20px rgba(255, 255, 255, 0.7);
            background: rgba(0, 0, 0, 0.5);
        }

        /* Section heading glow */
        h2 {
            text-align: center;
            text-shadow: 0 0 10px #ff0080, 0 0 20px #ff8000, 0 0 30px #00ffcc;
        }

        /* Paragraph styling */
        p {
            line-height: 1.6;
            text-align: justify;
        }

        /* Smooth scroll */
        html {
            scroll-behavior: smooth;
        }
    </style>
</head>
<body>
    <!-- Insert the image -->
    <img src="c:\Users\sudharshan\Downloads\pain.jpg" alt="Akatsuki Characters" usemap="#akatsukiMap" width="1536" height="768">

    <!-- Define the image map -->
    <map name="akatsukiMap">
        <area shape="rect" coords="0,0,192,768" alt="Character 1" href="#character1">
        <area shape="rect" coords="192,0,384,768" alt="Character 2" href="#character2">
        <area shape="rect" coords="384,0,576,768" alt="Character 3" href="#character3">
        <area shape="rect" coords="576,0,768,768" alt="Character 4" href="#character4">
        <area shape="rect" coords="768,0,960,768" alt="Character 5" href="#character5">
        <area shape="rect" coords="960,0,1152,768" alt="Character 6" href="#character6">
        <area shape="rect" coords="1152,0,1344,768" alt="Character 7" href="#character7">
        <area shape="rect" coords="1344,0,1536,768" alt="Character 8" href="#character8">
    </map>

    <!-- Define sections for each character -->
    <div id="character1">
        <h2>Character 1: Sasori</h2>
        <p>Role: Puppet master and artist.<br>
        Abilities: Mastery in puppet-making; turns humans into puppets to preserve their abilities.<br>
        Backstory: Left the Sand Village after becoming disillusioned with life and death.<br>
        Goal: Eternal existence through his puppets.</p>
    </div>
    <div id="character2">
        <h2>Character 2</h2>
        <p>. Kakuzu
            Role: Partner of Hidan; financial overseer of Akatsuki.
            Abilities:
            Earth Grudge Fear: Threads within his body allow him to steal hearts and extend his life.
            Possesses five hearts, each using a different elemental chakra.
            Backstory: Former Hidden Waterfall ninja who was exiled after a failed assassination.
            Goal: Accumulate wealth and power.</p>
    </div>
    <div id="character3">
        <h2>Character 3</h2>
        <p>Itachi Uchiha
            Role: Member; former ANBU captain of the Leaf Village.
            Abilities:
            Sharingan and Mangekyō Sharingan: Master of genjutsu, including the deadly Tsukuyomi.
            Amaterasu (black flames) and Susanoo.
            Backstory: Sacrificed his reputation and life to protect Konoha by eliminating the Uchiha clan under orders.
            Goal: Spy on Akatsuki and ensure the safety of his brother, Sasuke.</p>
    </div>
    <div id="character4">
        <h2>Character 4</h2>
        <p> Konan
            Role: Co-founder and second-in-command.
            Abilities:
            Paper Ninjutsu: Manipulates countless paper sheets, often infused with explosive tags.
            Creates intricate and deadly origami techniques.
            Backstory: A loyal friend of Nagato, deeply affected by the violence of war.
            Goal: Support Nagato's vision for peace.</p>
    </div>
    <div id="character5">
        <h2>Character 5</h2>
        <p> Pain (Nagato)
            Role: Leader (de facto)
            Abilities:
            Wields the Rinnegan, granting mastery over all chakra natures.
            Uses the Six Paths of Pain, controlling six corpses, each representing a unique ability (e.g., summoning, absorption).
            Backstory: A former student of Jiraiya, Nagato formed Akatsuki to bring peace to the world but was corrupted by war and pain.
            Goal: Enforce peace through fear and control of powerful weapons.</p>
    </div>
    <div id="character6">
        <h2>Character 6</h2>
        <p>Tobi (Obito Uchiha)
            Role: Initially a comical member, later revealed as the mastermind.
            Abilities:
            Sharingan with Kamui for space-time manipulation.
            Later controls the Ten-Tails as its Jinchūriki.
            Backstory: Presumed dead, Obito was saved by Madara Uchiha and manipulated into his plans.
            Goal: Enact the Eye of the Moon Plan to create a false utopia through genjutsu.</p>
    </div>
    <div id="character7">
        <h2>Character 7</h2>
        <p>Kisame Hoshigaki
            Role: Partner of Itachi.
            Abilities:
            Wields Samehada, a living sword that absorbs chakra.
            Massive chakra reserves and water-based jutsu like Water Prison Shark Dance Technique.
            Backstory: A former Mist ninja, betrayed his comrades to protect secrets.
            Goal: Achieve Akatsuki's mission of power and world control.</p>
    </div>
    <div id="character8">
        <h2>Character 8</h2>
        <p>Deidara
            Role: Explosives expert and artist.
            Abilities:
            Explosive Clay: Shapes and detonates clay using special mouths in his palms.
            Signature attack: C4 Karura creates microscopic bombs to destroy targets at the cellular level.
            Backstory: A rogue ninja from the Stone Village, obsessed with art and destruction.
            Goal: Prove that his explosive art is the ultimate form of expression.</p>
    </div>
    <div id="character8">
        <h2>Character 9</h2>
        <p>Orochimaru (Former Member)
            Role: Rogue ninja and scientist.
            Abilities:
            Mastery of forbidden jutsu and body modification.
            Seeks immortality through body transfers.
            Backstory: Left Akatsuki after failing to take Itachi's body.
            Goal: Gain ultimate knowledge and eternal life.</p>
</body>
</html>

# OUTPUT![Screenshot 2024-11-29 100329](https://github.com/user-attachments/assets/7b9c42c4-ed4d-4de6-b14e-fa7d88442511)

![Screenshot 2024-11-29 100339](https://github.com/user-attachments/assets/f4017d41-7729-4a59-98bc-667c4b7f7866)
![Screenshot 2024-11-29 100348](https://github.com/user-attachments/assets/9e642bd5-80a5-4f14-ba80-72764fbd8543)
![Screenshot 2024-11-29 100356](https://github.com/user-attachments/assets/71668839-5767-4137-b0b9-50670199dc98)

# RESULT
The program for implementing image maps using HTML is executed successfully.
