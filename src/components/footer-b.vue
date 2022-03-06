<template>
     <footer class="footer ">
        <div class="footer-container flex">
            <div class="footer-logo">
                <h2 class="color" >Sharingan</h2>
                <p class="color">Copyright © 2020</p>
            </div>
            <nav class="footer-nav"> 
                <ul class="color">
                    <li><a href="#">Semesters</a> </li>
                   
                    <li><a href="#">About Us</a></li>
                </ul>
            </nav>
            <div class="social">
               <a href="">
                   <i class="fab fa-facebook fa-2x"></i>
               </a>
               <a href="">
                   <i class="fab fa-instagram fa-2x"></i>
               </a>
               <a href="">
                   <i class="fab fa-twitter fa-2x"></i>
               </a>
            </div>
        </div>

    </footer>
</template>

<style >
.footer {
  display: block;
  height: 166px;
  background-color: var(--primary-color);
}

.footer-container{
    justify-content: space-evenly;
}
.footer a{
  color: #fff;
}

.footer-logo{
    margin-top: 44px;
}
.footer-nav{
    margin-top: 48px;
}

.social{
    margin-top: 58px;
}
.social a {
  margin: 0 5px;
  color: #fff;
}
.social a i {
    color: #fff;
}
</style>