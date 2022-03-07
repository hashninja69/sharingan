<template>
  <section class="showcase">
    <div class="showcase-container flex">
      <div class="showcase-text flex">
        <h1>Sharingan</h1>
        <p>
          This website is created for BCA students for right now, here they can
          get their notes, practical files and question papers. And there is one
          more thing that is the community, after joinning community you can
          contribute in developing some features for this website .
        </p>
        <div class="showcase-btn">
          <a href="#/about">About Us</a>
        </div>
      </div>
      <div class="showcase-form">
        <div class="card">
          <h2>Join the community</h2>
          <form action="">
            <div class="form-control">
              <input type="text" name="name" placeholder="Name" required />
            </div>
            <div class="form-control">
              <input type="email" name="email" placeholder="Email" required />
            </div>
            <input type="submit" value="Send" class="btn btn-primary" />
          </form>
        </div>
      </div>
    </div>
  </section>

  <section class="feature">
    <div class="feature-container">
      <h2 class="feature-heading text-center">More interesting things</h2>
      <p class="text-center">
        Instead of using the Turbo C++ compiler.It is better to use the Visual
        Studio Code it is a source code editor made by Microsoft for Windows,
        Linux and macOS. But to build C/C++ programs it require a GCC Compiler
        in it, which is needed to be downloaded and installed additionaly.
      </p>
      <h2 class="text-center paddingtop">Download</h2>
    </div>

    <div class="download flex margintop">
      <a
        class="btn btn-outline"
        href="https://sourceforge.net/projects/mingw-w64/files/Toolchains%20targetting%20Win32/Personal%20Builds/mingw-builds/installer/mingw-w64-install.exe/download"
      >
        <img class="imgsize" src="../assets/images/mingw64.svg" alt="mingw64" />
      </a>
      <a class="btn btn-outline" href="https://code.visualstudio.com/download">
        <img class="imgsize" src="../assets/images/vscode.png" alt="VS Code" />
      </a>
    </div>

    <div class="heading flex">
      <h3 class="heading">Mingw-w64</h3>
      <h3 class="heading">VS Code</h3>
    </div>
  </section>
</template>


<style>
.showcase {
  margin-top: 45px;
}
.showcase-container {
  background: var(--primary-color);

  color: #fff;
  justify-content: center;
  height: 425px;
}

.showcase-text {
  width: 50%;
  flex-direction: column;

  padding: 20px 117px;

  margin-left: 28px;
  animation: slideInFromLeft 500ms ease-in;
}
.showcase-form {
  animation: slideInFromRight 500ms ease-in;
}

.showcase-text h1 {
  margin-top: 71px;
}

.showcase-text p {
  line-height: 1.6;
}
.showcase-btn {
  color: #fff;
  border: 1px solid white;
  border-radius: 9px;
  width: 88px;
  height: 33px;
  text-align: center;
  margin-top: 18px;
  background: #ad1f2a;
}

.showcase-btn:hover {
  transform: scale(1.2);
}

.showcase-btn a {
  color: #fff;
}

.showcase-form input[type="text"],
.showcase-form input[type="email"] {
  width: 100%;
  font-size: 16px;
  border-width: 0px 0px 1px;

  border-bottom: 1px solid rgb(180, 190, 203);
  padding: 3px;
}
.form-control {
  margin: 31px 0;
}

.showcase::before,
.showcase::after {
  content: "";
  position: absolute;
  height: 86px;
  top: 425px;
  right: 0px;
  left: 0px;
  transform: skewY(-3deg);
  background: white;
}

.feature {
  padding-top: 36px;
  animation: slideInFromBottom 500ms ease-in;
}
.feature-heading {
  max-width: 272px;
  margin: auto;
}

.feature p {
  width: 781px;
  margin: 0 auto;
}

.paddingtop {
  padding-top: 12px;
}

.margintop {
  margin-top: 11px;
}
.imgsize {
  width: 77px;
  margin: 0 5px;
}
.heading {
  margin: 0 36px;
  margin-bottom: 24px;
  justify-content: center;
}

.download {
  justify-content: center;
}

.card {
  background-color: white;
  z-index: 3;
  color: #333;
  border-radius: 10px;
  box-shadow: 0 3px 10px rgba(0, 0, 0, 0.2);
  padding: 20px;
  margin-top: 51px;
  height: 266px;
  width: 360px;
}

.card h2 {
  font-weight: lighter;
}
.btn {
  display: inline-block;
  padding: 10px 30px;
  cursor: pointer;
  background-color: var(--primary-color);
  color: #fff;
  border: none;
  border-radius: 5px;
}

.btn-outline {
  background-color: transparent;
  border: 1px solid #fff;
}

.btn:hover {
  transform: scale(0.95);
}

.text-center {
  text-align: center;
}

.color {
  color: #fff;
}

.dropdown-content::-webkit-scrollbar {
  display: none;
}

@media (max-width: 900px) {
  .showcase-text {
    padding: 2px 36px;
    width: 100%;
    margin: auto;
    margin-top: 175px;
  }
  .showcase-text h1 {
    margin-top: 0px;
  }
  .showcase-container {
    flex-direction: column;
    height: 643px;
  }
  .showcase::before,
  .showcase::after {
    height: 58px;
    top: 390px;
  }
  .card {
    margin: 62px auto;
  }
  .showcase-form {
    background-color: #fff;
    margin-top: 58px;
  }
  .feature-heading {
    margin-top: 26px;
  }

  .feature p {
    width: 454px;
    text-align: center;
  }
}

@media (max-width: 400px) {
  .showcase-container {
    height: 431px;
  }

  .showcase-form {
    margin-top: 0px;
    height: 66px;
  }

  .showcase-text {
    margin-top: 30px;
  }
  .showcase::before,
  .showcase::after {
    top: 395px;
    height: 49px;
  }

  .card {
    margin: 45px auto;
    width: 283px;
    box-shadow: 0 3px 10px rgb(0 0 0);
  }
  .feature-heading {
    margin-top: 226px;
  }
  .feature p {
    width: 100%;
  }
  .heading {
    margin: 0 24px;
    font-size: 22px;
  }
}
</style>