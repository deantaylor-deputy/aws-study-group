```bash
# Update the system
sudo apt update

# Install Apache
sudo apt install -y apache2

# Start Apache service
sudo systemctl start apache2

# Enable Apache to start on boot (optional in a container, but good practice)
sudo systemctl enable apache2

# Check Apache status
systemctl status apache2

# Create a simple HTML page
sudo tee /var/www/html/index.html > /dev/null <<EOF
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Welcome to My EC2 Test</title>
</head>
<body>
    <h1>Welcome to My EC2 Demo</h1>
    <p>Current time: <span id="time"></span></p>

    <script>
        function updateTime() {
            document.getElementById('time').textContent = new Date().toLocaleString();
        }
        updateTime();
        setInterval(updateTime, 1000);
    </script>
</body>
</html>
EOF

# Restart Apache to ensure all changes are applied
sudo systemctl restart apache2

```
