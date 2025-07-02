# From-
I'm creating a online form 
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Ashok Enterprise Form</title>
  <style>
    body {
      font-family: Arial;
      background: #f2f2f2;
    }

    .form-box {
      width: 400px;
      margin: 50px auto;
      background: #fff;
      padding: 30px;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }

    h2 {
      color: #c00000;
      text-align: center;
    }

    label {
      margin-top: 15px;
      display: block;
      font-weight: bold;
    }

    input {
      width: 100%;
      padding: 8px;
      margin-top: 5px;
      border: 1px solid #ccc;
      border-radius: 5px;
    }

    button {
      margin-top: 20px;
      width: 100%;
      background-color: #d40000;
      color: white;
      padding: 10px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }

    .success {
      color: green;
      text-align: center;
      margin-top: 15px;
    }
  </style>
</head>
<body>
  <div class="form-box">
    <h2>Ashok Enterprise Form</h2>
    <form action="upload.php" method="POST" enctype="multipart/form-data">
      <label for="name">Name</label>
      <input type="text" name="name" required />

      <label for="phone">Phone</label>
      <input type="text" name="phone" required pattern="[0-9]{10}" />

      <label for="email">Email</label>
      <input type="email" name="email" required />

      <label for="document">Upload Document</label>
      <input type="file" name="document" accept=".pdf,.jpg,.png,.jpeg" required />

      <button type="submit">Submit</button>
    </form>
  </div>
</body>
</html>
