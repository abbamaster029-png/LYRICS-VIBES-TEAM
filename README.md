<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>Lyrics Vibes Team | Member Profile</title>

  <style>
    @import url('https://fonts.googleapis.com/css2?family=Cinzel:wght@500;600;700&family=Montserrat:wght@400;500;600;700&display=swap');

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      min-height: 100vh;
      background:
        radial-gradient(circle at top, #12366d 0%, #071a38 45%, #020b1d 100%);
      color: #fff;
      font-family: 'Montserrat', sans-serif;
      padding: 28px 14px;
    }

    .page {
      width: 100%;
      max-width: 520px;
      margin: auto;
    }

    /* TEAM NAME */

    .header {
      text-align: center;
      margin-bottom: 22px;
    }

    .header-line {
      width: 75px;
      height: 2px;
      background: #d9ad32;
      margin: 0 auto 12px;
      box-shadow: 0 0 10px #d9ad32;
    }

    .team-name {
      font-family: 'Cinzel', serif;
      color: #e4b83f;
      font-size: clamp(24px, 7vw, 34px);
      font-weight: 700;
      letter-spacing: 1.5px;
      text-align: center;
    }

    .subtitle {
      margin-top: 7px;
      color: #eadcae;
      font-size: 11px;
      letter-spacing: 3px;
      text-align: center;
    }

    /* MAIN CARD */

    .card {
      position: relative;
      background: rgba(7, 27, 57, 0.94);
      border: 1px solid #d9ad32;
      border-radius: 24px;
      padding: 28px 20px 24px;
      box-shadow:
        0 0 25px rgba(217, 173, 50, 0.08),
        inset 0 0 35px rgba(0, 0, 0, 0.18);
    }

    .card::before {
      content: "";
      position: absolute;
      inset: 7px;
      border: 1px solid rgba(217, 173, 50, 0.22);
      border-radius: 19px;
      pointer-events: none;
    }

    /* PROFILE ICON */

    .profile-icon {
      width: 92px;
      height: 92px;
      margin: 0 auto 18px;
      border-radius: 50%;
      border: 2px solid #e4b83f;
      display: flex;
      align-items: center;
      justify-content: center;
      background: #061b3b;
      box-shadow: 0 0 18px rgba(228, 184, 63, 0.25);
      position: relative;
    }

    .profile-icon::before {
      content: "♙";
      font-size: 55px;
      color: #e4b83f;
      transform: rotate(180deg);
    }

    /* NAME */

    .member-name {
      text-align: center;
      font-family: 'Cinzel', serif;
      font-size: clamp(21px, 6vw, 29px);
      line-height: 1.25;
      font-weight: 700;
      color: #fff;
      margin-bottom: 14px;
    }

    /* POSITION */

    .position {
      width: fit-content;
      margin: auto;
      background: linear-gradient(135deg, #e7bd4c, #c99820);
      color: #071a38;
      padding: 8px 28px;
      border-radius: 30px;
      font-weight: 700;
      font-size: 14px;
      letter-spacing: 1px;
      box-shadow: 0 5px 18px rgba(217, 173, 50, 0.15);
    }

    /* DIVIDER */

    .divider {
      display: flex;
      align-items: center;
      gap: 10px;
      margin: 22px auto;
      max-width: 280px;
    }

    .divider span {
      height: 1px;
      flex: 1;
      background: #d9ad32;
      opacity: 0.7;
    }

    .diamond {
      width: 9px;
      height: 9px;
      background: #d9ad32;
      transform: rotate(45deg);
    }

    /* MEMBER ID */

    .member-id {
      border: 1px solid rgba(217, 173, 50, 0.75);
      border-radius: 12px;
      padding: 12px;
      text-align: center;
      color: #e4b83f;
      font-size: 14px;
      font-weight: 600;
      letter-spacing: 1px;
      margin-bottom: 24px;
    }

    /* PRIVATE SECTION */

    .private-box {
      border: 1px solid #d9ad32;
      border-radius: 18px;
      padding: 20px 16px;
      background: rgba(2, 14, 34, 0.55);
    }

    .lock {
      width: 48px;
      height: 48px;
      margin: -42px auto 12px;
      background: #071a38;
      border: 1px solid #d9ad32;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 23px;
    }

    .private-title {
      text-align: center;
      color: #e4b83f;
      font-family: 'Cinzel', serif;
      font-size: 16px;
      font-weight: 600;
      letter-spacing: 1px;
      margin-bottom: 16px;
    }

    input {
      width: 100%;
      height: 48px;
      border-radius: 10px;
      border: 1px solid #c99e2d;
      background: #061a38;
      color: white;
      padding: 0 14px;
      outline: none;
      font-size: 14px;
    }

    input::placeholder {
      color: #9ca6b6;
    }

    input:focus {
      border-color: #f0c94f;
      box-shadow: 0 0 10px rgba(228, 184, 63, 0.18);
    }

    button {
      width: 100%;
      height: 48px;
      margin-top: 11px;
      border: none;
      border-radius: 10px;
      background: linear-gradient(135deg, #edc34c, #c79620);
      color: #071a38;
      font-size: 13px;
      font-weight: 700;
      letter-spacing: 0.5px;
      cursor: pointer;
    }

    button:active {
      transform: scale(0.98);
    }

    .error {
      display: none;
      color: #ff8585;
      text-align: center;
      font-size: 12px;
      margin-top: 10px;
    }

    /* PRIVATE DETAILS */

    .private-info {
      display: none;
      margin-top: 17px;
      border-top: 1px solid rgba(217, 173, 50, 0.4);
      padding-top: 15px;
    }

    .info-item {
      padding: 9px 0;
      border-bottom: 1px solid rgba(255,255,255,0.08);
      font-size: 13px;
      line-height: 1.5;
    }

    .info-item:last-child {
      border-bottom: none;
    }

    .info-item strong {
      display: block;
      color: #e4b83f;
      font-size: 11px;
      text-transform: uppercase;
      letter-spacing: 0.7px;
      margin-bottom: 2px;
    }

    .info-item span {
      color: #e8edf5;
    }

    /* FOOTER */

    .footer {
      text-align: center;
      margin-top: 18px;
      color: #c9a83d;
      font-size: 10px;
      letter-spacing: 2px;
    }

    /* SMALL PHONES */

    @media (max-width: 360px) {

      body {
        padding: 20px 10px;
      }

      .card {
        padding: 24px 15px 20px;
      }

      .profile-icon {
        width: 78px;
        height: 78px;
      }

      .profile-icon::before {
        font-size: 45px;
      }

      .private-box {
        padding: 18px 12px;
      }

      .team-name {
        font-size: 22px;
      }
    }
  </style>
</head>

<body>

  <main class="page">

    <!-- HEADER -->

    <header class="header">

      <div class="header-line"></div>

      <h1 class="team-name">
        LYRICS VIBES TEAM
      </h1>

      <p class="subtitle">
        OFFICIAL MEMBER PROFILE
      </p>

    </header>


    <!-- PROFILE CARD -->

    <section class="card">

      <!-- Profile icon -->
      <div class="profile-icon"></div>


      <!-- Public information -->

      <h2 class="member-name">
        MUNAZZAFA SALISU UMAR
      </h2>

      <div class="position">
        ADMIN
      </div>


      <div class="divider">
        <span></span>
        <div class="diamond"></div>
        <span></span>
      </div>


      <div class="member-id">
        MEMBER ID: LVT004
      </div>


      <!-- Private information -->

      <div class="private-box">

        <div class="lock">
          🔒
        </div>

        <h3 class="private-title">
          PRIVATE INFORMATION
        </h3>

        <input
          type="password"
          id="password"
          placeholder="Enter password"
        >

        <button onclick="unlockInfo()">
          VIEW PRIVATE INFORMATION
        </button>

        <div class="error" id="error">
          Incorrect password. Please try again.
        </div>


        <!-- Hidden information -->

        <div class="private-info" id="privateInfo">

          <div class="info-item">
            <strong>Username</strong>
            <span>M Sayyada Lyrics</span>
          </div>

          <div class="info-item">
            <strong>Phone Number</strong>
            <span>08102390873</span>
          </div>

          <div class="info-item">
            <strong>Email Address</strong>
            <span>msayyadalyrics@gmail.com</span>
          </div>

          <div class="info-item">
            <strong>Age</strong>
            <span>20</span>
          </div>

          <div class="info-item">
            <strong>Country</strong>
            <span>Nigeria</span>
          </div>

          <div class="info-item">
            <strong>Section</strong>
            <span>All of them</span>
          </div>

          <div class="info-item">
            <strong>Competition Experience</strong>
            <span>No</span>
          </div>

          <div class="info-item">
            <strong>Why She Joined</strong>
            <span>
              Because I love lyrics, and I really admire
              the LYRICS VIBES TEAM. I also enjoy
              interacting and connecting with its members.
            </span>
          </div>

          <div class="info-item">
            <strong>About Her</strong>
            <span>
              I am from Kano, Nigeria. I enjoy interacting
              with people like me, and I am a calm person
              who doesn't like unnecessary drama or noise.
            </span>
          </div>

        </div>

      </div>

    </section>


    <footer class="footer">
      LYRICS VIBES TEAM
    </footer>

  </main>


  <script>

    function unlockInfo() {

      const password =
        document.getElementById("password").value;

      const privateInfo =
        document.getElementById("privateInfo");

      const error =
        document.getElementById("error");


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