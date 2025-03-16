<!DOCTYPE html>
<lang="en">
<head>
    <meta charset="utf-8">
    </spanPurple><title>Test</title>
</head>

<body>
    <spanPurple><h3>Hallo Stephan</h3></spanPurple>
        <div>Wie versprochen schicke schicke ich dir den Link vom Restaurant in Bern, wovon ich dir erzählt habe. 
            <br> <br> Jetzt ist es nur leider so, dass ich mir Visual Studio heruntergeladen habe und ein bisschen mit HTML herumspiele.
            <br> Daher kann ich dir den Namen des Restaurants nicht einfach verraten, sondern du musst zuerst das folgende Rätsel richtig lösen.

            <br> <br><spanGreen><strong>Viel Erfolg!</strong></spanGreen>

            <div class="raetsel">
            <br> Ich habe Blätter, bin aber kein Baum.
            <br> Ich kann dir einiges beibringen, doch ich spreche nicht.
            <br> Manchmal bin ich dünn, manchmal dick.
            <br> Was bin ich?
        </div>
        </div>

    <br><br><Strong>Tipp:</Strong> Die Lösung besteht aus nur einem Wort.

   <br><br> <p>   
    Textfeld: <input type="text"
            id="Textfeld"
            placeholder="Lösung eingeben">
        </p>


    <p>
        <button
        onclick="myFunction()">Antwort prüfen</button>
        </p>

        <div id="errorMessage" class="error-message">Falsches Passwort. <br> Versuch's nochmal in <strong> Kleinbuchstaben</strong>.</div>
    




<script>
            function myFunction() {
                const password = document.getElementById("Textfeld").value;
                const correctPassword = "buch";
                const errorMessage = document.getElementById("errorMessage");

                if (password === correctPassword) {
                    errorMessage.style.display = "none";
                    window.open("https://www.levivant.ch");
                } else {

                    errorMessage.style.display = "block";
                }
                
            }

</script>

    


</body>
</html>


<style>
    spanPurple {
        color: purple;
    }

    spanGreen {
        color: green;
    }

    .error-message {
        color: red;
        border: 1px solid red;
        padding: 5px;
        margin-top: 10px;
        display: none;
    }

    .raetsel {
        margin-left: 100px;
    }
</style>
