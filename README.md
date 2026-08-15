<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>Lyrics Vibes Team - Member Profile</title>

  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
    }

    body {
      min-height: 100vh;
      background: linear-gradient(145deg, #061a3a, #0b2d5c);
      color: white;
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 25px;
    }

    .profile-card {
      width: 100%;
      max-width: 430px;
      background: #09244a;
      border: 1px solid #d4af37;
      border-radius: 20px;
      padding: 30px 22px;
      text-align: center;
      box-shadow: 0 10px 35px rgba(0,0,0,0.35);
    }

    .team-name {
      color: #d4af37;
      font-size: 25px;
      font-weight: bold;
      letter-spacing: 1px;
      margin-bottom: 5px;
    }

    .subtitle {
      color: #dcdcdc;
      font-size: 13px;
      margin-bottom: 28px;
    }

    .member-name {
      font-size: 24px;
      font-weight: bold;
      margin-bottom: 12px;
    }

    .position {
      display: inline-block;
      color: #061a3a;
      background: #d4af37;
      padding: 7px 20px;
      border-radius: 30px;
      font-weight: bold;
      margin-bottom: 15px;
    }

    .member-id {
      color: #d4af37;
      font-size: 15px;
      margin-bottom: 30px;
    }

    .private-box {
      border-top: 1px solid #d4af37;
      padding-top: 22px;
    }

    .private-title {
      color: #d4af37;
      font-size: 18px;
      margin-bottom: 15px;
    }

    input {
      width: 100%;
      padding: 13px;
      border-radius: 10px;
      border: 1px solid #777;
      outline: none;
      margin-bottom: 12px;
      font-size: 15px;
    }

    button {
      width: 100%;
      padding: 13px;
      border: none;
      border-radius: 10px;
      background: #d4af37;
      color: #061a3a;
      font-size: 15px;
      font-weight: bold;
      cursor: pointer;
    }

    button:hover {
      opacity: 0.9;
    }

    .private-info {
      display: none;
      text-align: left;
      margin-top: 20px;
      background: #061a3a;
      border: 1px solid #d4af37;
      border-radius: 12px;
      padding: 18px;
    }

    .private-info p {
      margin-bottom: 12px;
      line-height: 1.5;
    }

    .private-info strong {
      color: #d4af37;
    }

    .error {
      color: #ff7777;
      margin-top: 10px;
      display: none;
      font-size: 14px;
    }
  </style>
</head>

<body>

  <div class="profile-card">

    <div class="team-name">LYRICS VIBES TEAM</div>

    <div class="subtitle">
      OFFICIAL MEMBER PROFILE
    </div>

    <div class="member-name">
      MUNAZZAFA SALISU UMAR
    </div>

    <div class="position">
      ADMIN
    </div>

    <div class="member-id">
      MEMBER ID: LVT004
    </div>

    <div class="private-box">

      <div class="private-title">
        🔐 Private Information
      </div>

      <input
        type="password"
        id="password"
        placeholder="Enter password"
      >

      <button onclick="unlockInfo()">
        VIEW PRIVATE INFORMATION
      </button>

      <div class="error" id="error">
        Incorrect password.
      </div>

      <div class="private-info" id="privateInfo">

        <p>
          <strong>Username:</strong>
          M Sayyada Lyrics
        </p>

        <p>
          <strong>Phone Number:</strong>
          08102390873
        </p>

        <p>
          <strong>Email:</strong>
          msayyadalyrics@gmail.com
        </p>

        <p>
          <strong>Age:</strong>
          20
        </p>

        <p>
          <strong>Country:</strong>
          Nigeria
        </p>

        <p>
          <strong>Section:</strong>
          All of them
        </p>

        <p>
          <strong>Competition Experience:</strong>
          No
        </p>

        <p>
          <strong>Why she joined:</strong><br>
          Because I love lyrics, and I really admire the
          LYRICS VIBES TEAM. I also enjoy interacting and
          connecting with its members.
        </p>

        <p>
          <strong>About her:</strong><br>
          I am from Kano, Nigeria. I enjoy interacting with
          people like me, and I am a calm person who doesn't
          like unnecessary drama or noise.
        </p>

      </div>

    </div>

  </div>

  <script>
    function unlockInfo() {

      const password = document.getElementById("password").value;
      const privateInfo = document.getElementById("privateInfo");
      const error = document.getElementById("error");

      if (password === "Sayyada2003@") {

        privateInfo.style.display = "block";
        error.style.display = "none";

      } else {

        privateInfo.style.display = "none";
        error.style.display = "block";

      }
    }
  </script>

</body>
</html>