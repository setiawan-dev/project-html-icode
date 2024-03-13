# project-html-icode


<button type="button" class="my-btn my-btn-success">Success</button>


.my-btn {
  display: inline-block;
  padding: 0.5rem 1rem;
  font-size: 1rem;
  font-weight: 400;
  line-height: 1.5;
  text-align: center;
  text-decoration: none;
  vertical-align: middle;
  cursor: pointer;
  user-select: none;
  border: 1px solid transparent;
  border-radius: 0.25rem;
  transition: color 0.15s ease-in-out, background-color 0.15s ease-in-out, border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out;
}

.my-btn-success {
  color: #fff;
  background-color: #28a745;
  border-color: #28a745;
}

.my-btn-success:hover {
  color: #fff;
  background-color: #1e7e34;
  border-color: #1c7430;
}

.my-btn-success:focus, .my-btn-success.focus {
  box-shadow: 0 0 0 0.2rem rgba(40, 167, 69, 0.5);
}

.my-btn-success:active, .my-btn-success.active, .my-btn-success.pressed {
  color: #fff;
  background-color: #1e7e34;
  border-color: #1c7430;
  box-shadow: 0 0 0 0.2rem rgba(40, 167, 69, 0.5);
}


<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="style.css">
  <title>Hotel Listings</title>
</head>
<body>
  <main class="hotel-list">
    <section class="hotel-item">
      <img src="https://images.unsplash.com/photo-1455587734955-081b22074882?q=80&w=1470&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="Hotel 1" class="hotel-image">
      <div class="hotel-content">
        <h2 class="hotel-heading">Hotel 1 - Luxury Retreat</h2>
        <p class="hotel-description">
          Hotel 1 is a luxury retreat nestled in the heart of the city. With its stunning architecture, impeccable service, and world-class amenities, it offers an unforgettable experience for discerning travelers.
        </p>
      </div>
    </section>

    <section class="hotel-item">
      <img src="https://images.unsplash.com/photo-1455587734955-081b22074882?q=80&w=1470&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="Hotel 2" class="hotel-image">
      <div class="hotel-content">
        <h2 class="hotel-heading">Hotel 2 - Urban Oasis</h2>
        <p class="hotel-description">
          Hotel 2 is an urban oasis that combines style, comfort, and convenience. Located in a vibrant neighborhood, it offers easy access to the city's top attractions, along with cozy rooms, friendly staff, and a range of amenities.
        </p>
      </div>
    </section>

    <section class="hotel-item">
      <img src="https://images.unsplash.com/photo-1455587734955-081b22074882?q=80&w=1470&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="Hotel 3" class="hotel-image">
      <div class="hotel-content">
        <h2 class="hotel-heading">Hotel 3 - Seaside Serenity</h2>
        <p class="hotel-description">
          Hotel 3 is a seaside sanctuary that offers breathtaking views, serene surroundings, and a relaxed atmosphere. With its spacious rooms, delicious cuisine, and attentive service, it's the perfect place to unwind and recharge.
        </p>
      </div>
    </section>
  </main>
</body>
</html>


* {
  box-sizing: border-box;
}

body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
}

.hotel-list {
  display: inline-block;
  flex-wrap: wrap;
  justify-content: space-between;
  margin: 10px 20%;
}

.hotel-item {
  background-color: #f2f2f2;
  border-radius: 5px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  flex-basis: calc(33.333% - 1rem);
  margin-bottom: 1rem;
  overflow: hidden;
  display: flex;
}

.hotel-image {
  width: 80%;
  height: 250px;
  object-fit: cover;
}

.hotel-content {
  padding: 1rem;
  width: 60%;
}

.hotel-heading {
  font-size: 1.5rem;
  margin-top: 0;
  margin-bottom: 0.5rem;
}

.hotel-description {
  font-size: 0.9rem;
  line-height: 1.5;
  margin-bottom: 0;
}


<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="style.css">
  <title>Registration and Contact</title>
</head>
<body>
  <section class="registration">
    <h2 class="section-heading">Registration</h2>
    <form class="registration-form">
      <label for="name">Name:</label>
      <input type="text" id="name" name="name" required>

      <label for="email">Email:</label>
      <input type="email" id="email" name="email" required>

      <label for="password">Password:</label>
      <input type="password" id="password" name="password" required>

      <button type="submit" class="btn">Register</button>
    </form>
  </section>

  <section class="contact">
    <h2 class="section-heading">Contact Us</h2>
    <p class="contact-info">
      Phone: (123) 456-7890<br>
      Email: info@example.com<br>
      Address: 123 Example Street, Example City, EX 12345
    </p>
    <form class="contact-form">
      <label for="name">Name:</label>
      <input type="text" id="name" name="name" required>

      <label for="email">Email:</label>
      <input type="email" id="email" name="email" required>

      <label for="message">Message:</label>
      <textarea id="message" name="message" rows="5" cols="30" required></textarea>

      <button type="submit" class="btn">Send Message</button>
    </form>
  </section>
</body>
</html>

* {
  box-sizing: border-box;
}

body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
}

.section-heading {
  font-size: 2rem;
  margin-top: 2rem;
  margin-bottom: 1rem;
  text-align: center;
}

.registration, .contact {
  background-color: #f2f2f2;
  border-radius: 5px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  margin: 0 1rem;
  padding: 2rem;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}

.registration-form, .contact-form {
  width: 45%;
  margin-top: 1rem;
}

.registration-form label, .contact-form label {
  display: block;
  font-size: 1.2rem;
  margin-bottom: 0.5rem;
}

.registration-form input, .contact-form input, .contact-form textarea {
  width: 100%;
  padding: 0.5rem;
  font-size: 1rem;
  border-radius: 5px;
  border: 1px solid #ccc;
  margin-bottom: 1rem;
}

.registration-form button, .contact-form button {
  background-color: #4CAF50;
  color: white;
  padding: 0.5rem 1rem;
  font-size: 1.2rem;
  border-radius: 5px;
  border: none;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.registration-form button:hover, .contact-form button:hover {
  background-color: #3e8e41;
}

.contact-info {
  width: 45%;
  margin-top: 1rem;
  font-size: 1.2rem;
  line-height: 1.5;
} 
