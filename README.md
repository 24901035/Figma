# Ex09 Event Registration Web Application
## Date:16-11-2025

## AIM:
To design, develop and deploy a web application for event registration.

## DESIGN STEPS:

### Step 1:
Create a new frame.

### Step 2:
Select any one preset size of your choice.

### Step 3:
Select the shapes you need.

### Step 4:
Import images as needed.

### Step 5:
Create pages based on your need and link them.

### Step 6:

Validate the HTML and CSS code.

### Step 6:

Publish the website in the given URL.

## DESIGN TOOL:
Figma

## CODE:
LOGIN PAGE

```
<!DOCTYPE html>
<html>
<head>
  <title>Login Page</title>
  <style>
    body { font-family: Arial; background:#f2f2f2; padding:40px; }
    .container{ width:350px; margin:auto; background:white; padding:20px; border-radius:10px; }
    input{ width:100%; padding:10px; margin:10px 0; }
    button{ width:100%; padding:10px; background:#007bff; color:white; border:none; }
  </style>
</head>
<body>
<div class="container">
  <h2>Login</h2>
  <form action="events.html">
    <input type="text" placeholder="Username" required>
    <input type="password" placeholder="Password" required>
    <button type="submit">Login</button>
  </form>
</div>
</body>
</html>

```

EVENTS PAGE

```<!DOCTYPE html>
<html>
<head>
  <title>Events List</title>
  <style>
    body { font-family: Arial; padding:20px; }
    .event{ border:1px solid #ccc; padding:15px; margin:10px 0; border-radius:8px; }
    button{ background:#28a745; color:white; padding:8px 15px; border:none; }
  </style>
</head>
<body>

<h2>Available Events</h2>

<div class="event">
  <h3>Tech Expo 2025</h3>
  <p>Date: 25 Nov 2025</p>
  <a href="register.html?event=Tech Expo 2025"><button>Register</button></a>
</div>

<div class="event">
  <h3>AI Symposium</h3>
  <p>Date: 10 Dec 2025</p>
  <a href="register.html?event=AI Symposium"><button>Register</button></a>
</div>

</body>
</html>
```

REGISTER PAGE 

```
<!DOCTYPE html>
<html>
<head>
  <title>Event Registration</title>
  <style>
    body { font-family: Arial; padding:40px; background:#fafafa; }
    .container{ width:400px; margin:auto; background:white; padding:20px; border-radius:10px; }
    input{ width:100%; padding:10px; margin:10px 0; }
    button{ width:100%; padding:10px; background:#17a2b8; color:white; border:none; }
  </style>
</head>
<body>

<div class="container">
  <h2>Event Registration</h2>

  <form action="confirmation.html">
    <input type="text" placeholder="Full Name" required>
    <input type="email" placeholder="Email" required>
    <input type="text" placeholder="Phone Number" required>
    <button type="submit">Submit</button>
  </form>
</div>

<script>
  // Display event name on registration page (optional)
  const params = new URLSearchParams(window.location.search);
  const eventName = params.get("event");
  if (eventName) {
    document.querySelector("h2").innerText = "Register for: " + eventName;
  }
</script>

</body>
</html>
```

## OUTPUT:
![alt text](<Screenshot 2025-11-16 205000.png>)

![alt text](<Screenshot 2025-11-16 205013.png>)

![alt text](<Screenshot 2025-11-16 205025.png>)

## RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
