  <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Faculty Dashboard</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: Arial, sans-serif;
      display: flex;
      flex-direction: column;
      min-height: 100vh;
    }

    /* Header Styles */
    header {
      background-color: #2c3e50;
      color: white;
      padding: 1rem 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .logo {
      font-size: 1.5rem;
      font-weight: bold;
    }

    /* Navigation */
    nav {
      background-color: #34495e;
      padding: 1rem 2rem;
    }

    nav a {
      color: white;
      text-decoration: none;
      margin-right: 1rem;
    }

    nav a:hover {
      text-decoration: underline;
    }

    /* Main Content Container */
    .content-container {
      display: flex;
      flex: 1;
    }

    /* Sidebar Styles */
    .sidebar {
      width: 250px;
      background-color: #ecf0f1;
      padding: 2rem 1rem;
      border-right: 2px solid #bdc3c7;
    }

    .sidebar h3 {
      margin-bottom: 1.5rem;
      color: #2c3e50;
      text-align: center;
    }

    .sidebar ul {
      list-style: none;
    }

    .sidebar li {
      padding: 0.8rem 1rem;
      margin-bottom: 0.5rem;
      background-color: white;
      border-radius: 5px;
      cursor: pointer;
      transition: background-color 0.3s;
    }

    .sidebar li:hover {
      background-color: #3498db;
      color: white;
    }

    /* Main Content Styles */
    .main {
      flex: 1;
      padding: 2rem;
      background-color: #f8f9fa;
    }

    .main h1 {
      color: #2c3e50;
      margin-bottom: 0.5rem;
    }

    .main h2 {
      color: #7f8c8d;
      margin-bottom: 1.5rem;
      font-weight: normal;
    }

    .main p {
      margin-bottom: 1.5rem;
      line-height: 1.6;
    }

    /* Table Styles */
    table {
      width: 100%;
      border-collapse: collapse;
      background-color: white;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }

    th, td {
      padding: 1rem;
      text-align: left;
      border-bottom: 1px solid #ddd;
    }

    th {
      background-color: #34495e;
      color: white;
    }

    tr:hover {
      background-color: #f5f5f5;
    }

    /* Footer Styles */
    footer {
      background-color: #2c3e50;
      color: white;
      text-align: center;
      padding: 1rem;
      margin-top: auto;
    }
  </style>
</head>
<body>

  <!-- Header -->
  <header>
    <div class="logo">MRU Faculty Portal</div>
    <div>Welcome, User</div>
  </header>

  <!-- Navigation -->
  <nav>
    <a href="#">Home</a>
    <a href="#">About</a>
    <a href="#">Services</a>
    <a href="#">Contact</a>
  </nav>

  <!-- Main Content Container -->
  <div class="content-container">
    <!-- Sidebar -->
    <div class="sidebar">
      <h3>Menu</h3>
      <ul>
        <li>Dashboard</li>
        <li>Courses</li>
        <li>Settings</li>
        <li>Profile</li>
      </ul>
    </div>

    <!-- Main section -->
    <div class="main">
      <h1>Faculty of Science and Technology</h1>
      <h2>Muteesa Royal University</h2>
      <p>Below is a table containing simple course data:</p>

      <table>
        <tr>
          <th>Code</th>
          <th>Course Name</th>
          <th>Period</th>
        </tr>
        <tr>
          <td>BCS</td>
          <td>Computer Science</td>
          <td>3 Years</td>
        </tr>
        <tr>
          <td>BIT</td>
          <td>Information Technology</td>
          <td>3 Years</td>
        </tr>
        <tr>
          <td>DIT</td>
          <td>Diploma in Information Technology</td>
          <td>2 Years</td>
        </tr>
        <tr>
          <td>BEICT</td>
          <td>Bachelors of Education with ICT</td>
          <td>4 Years</td>
        </tr>
      </table>
    </div>
  </div>

  <!-- Footer -->
  <footer>
    &copy; <span id="year"></span> Muteesa Royal University 
  </footer>

  <script>
    // Automatically insert the current year in footer
    document.getElementById("year").textContent = new Date().getFullYear();
  </script>

</body>
</html>    
