# rotating-links
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Redirecting to WhatsApp</title>
</head>
<body>

    <script>
        var links = ["https://wa.me/60133322039", "https://wa.me/60175771517"];
        var linkIndex = 0;

        // Redirect to the first WhatsApp link immediately
        window.location.href = links[linkIndex];

        // Optionally, uncomment the following lines if you want to rotate links after a delay
        // setTimeout(function() {
        //     window.location.href = links[1];
        // }, 5000); // 5000 milliseconds (5 seconds) delay
    </script>

</body>
</html>

