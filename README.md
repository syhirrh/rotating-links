# rotating-links
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>WhatsApp Redirect</title>
</head>
<body>

    <script>
        var links = ["https://wa.me/60133322039", "https://wa.me/60175771517"];
        var linkIndex = 0;

        // Retrieve the last shown link index from local storage
        var lastLinkIndex = localStorage.getItem("lastLinkIndex");
        if (lastLinkIndex !== null) {
            linkIndex = parseInt(lastLinkIndex);
        }

        // Redirect to the current WhatsApp link
        window.location.href = links[linkIndex];

        // Rotate to the next link after a click
        document.body.addEventListener("click", function() {
            linkIndex = (linkIndex + 1) % links.length;
            localStorage.setItem("lastLinkIndex", linkIndex.toString());
            window.location.href = links[linkIndex];
        });
    </script>

</body>
</html>
