[styles.css](https://github.com/user-attachments/files/25379760/styles.css)
body {
  margin: 0;
  font-family: 'Arial', sans-serif;
  background-color: #fff0f5;
  color: #000000;
}
/* Header styles */
.header-container {
  display: flex;
  align-items: center;
  background-color: #d0e7f9;
  padding: 10px 20px;
  border-bottom: 2px solid #000;
}
.logo {
  width: 80px;
  height: auto;
  margin-right: 20px;
}
.header-text {
  flex: 1;
}
.school-name {
  font-family: 'Arial Rounded MT Bold', cursive, sans-serif;
  font-size: 1.8em;
  font-weight: bold;
  margin: 0;
  color: #000;
  animation: moveText 3s infinite alternate;
}
.address, .principal {
  margin: 5px 0 0 0;
  font-family: 'Arial', sans-serif;
  font-size: 0.9em;
  color: #000;
}
@keyframes moveText {
  0% { transform: translateX(0); }
  100% { transform: translateX(5px); }
}
/* Navigation styles */
nav {
  display: flex;
  justify-content: center;
  background-color: #ff69b4;
  position: sticky;
  top: 0;
  z-index: 1000;
}
nav ul {
  list-style: none;
  margin: 0;
  padding: 0;
  display: flex;
}
nav li {
  position: relative;
}
nav a {
  padding: 15px 20px;
  display: block;
  color: #e9e1e1;
  text-decoration: none;
  font-weight: bold;
  cursor: pointer;
}
nav a:hover {
  background-color: #ff69b4;
}
/* Dropdown styles */
.dropdown {
  display: none;
  position: absolute;
  top: 100%;
  left: 0;
  background-color: #ff69b4;
  min-width: 160px;
  z-index: 1;
}
.dropdown.show {
  display: block;
}
nav .dropdown a {
  padding: 12px 16px;
  display: block;
}
/* Main content styles */
section {
  padding: 40px 20px;
  max-width: 1000px;
  margin: auto;
}
#home {
  background-image: url('https://sghconcepts.com/wp-content/uploads/2017/08/Garden-City-High-School_120808-3795.jpg');
  background-size: cover;
  min-height: 400px;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  opacity: 0;
  animation: fadeInBackground 2s forwards;
}
#home h2 {
  background-color: rgba(153, 139, 139, 0.5);
  padding: 20px;
  border-radius: 10px;
}
section h2 {
  color: #da0c7a;
  margin-bottom: 20px;
  font-family: 'Cursive', sans-serif;
}
.about-dropdown {
  padding: 15px 20px;
  background-color: #ff69b4;
  color: #fff;
  border: none;
  font-weight: bold;
  cursor: pointer;
  font-size: 1em;
}
.gallery {
  display: flex;
  flex-wrap: wrap;
  gap: 15px;
  justify-content: center;
}
.gallery img {
  width: calc(25% - 10px);
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0,0,0,0.2);
}
footer {
  background-color: #ff69b4;
  color: #fff;
  text-align: center;
  padding: 15px 10px;
}
@media(max-width: 768px){
  .gallery img {
    width: calc(50% - 10px);
  }
}
/* Additional styles for staff page content, departments, contact info, etc. (same as in your original CSS) */
