<template>
      <section class="aboutus">
          <div class="aboutus_heading">
                <h2>About Us</h2>
                <p class="aboutus_para">Lorem ipsum dolor sit amet consectetur adipisicing elit. Excepturi dolorum atque optio ex modi distinctio consequuntur totam alias facilis voluptate quam veritatis iusto, labore, amet officia eligendi temporibus eius molestias.</p>
          </div>
          <h2 class="who_heading">Who We are</h2>
    </section>

     <div class="whoweare">
            <div class="imgcard">
                <img src="../about us/1.jpg" alt=""> 
                Manik</div>
            <div class="imgcard">
              <img src="../about us/2.jpg" alt="">
                Pratham              
            </div>
          
            <div class="imgcard">
              <img src="../about us/3.jpg" alt="">
            Shivansh
            </div>
            <div class="imgcard">
              <img src="../about us/3.jpg" alt="">
            Abhishek
            </div>
            <div class="imgcard">
              <img src="../about us/3.jpg" alt="">
            Sagar
            </div>
        </div>
        
        <div class="cheading">

          <h2 class="contactus_heading">Contact Us</h2>
          <h3 class="small_heading">Drop Us a mail to contribute or see our recent acitvities.</h3>
          <h5 class="email"><a href="#">sharingan@gmail.com</a></h5>
        </div>
        <section class="contactus">
            <a href="">
                <i class="fab fa-email fa-2x"></i>
            </a>
            <a href="">
                <i class="fab fa-facebook fa-2x"></i>
            </a>
            <a href="">
                <i class="fab fa-instagram fa-2x"></i>
            </a>
            <a href="">
                <i class="fab fa-twitter fa-2x"></i>
            </a>
        </section>
</template>

<style scoped>
.aboutus{
    margin-top: 88px;
    display: flex;
    flex-direction: column;
    align-items: center;
  animation: slideInFromTop 500ms ease-in;
   
}
.aboutus_heading{
    text-align: center;
}

.aboutus_para{
    text-align: center;
    line-height: 1.3;
    width: 800px;
}

.who_heading{
    margin-bottom: 12px;
}
.whoweare{
    display: flex;
    justify-content: center;
    text-align: center;
    /* flex-direction: row; */
  animation: slideInFromRight 500ms ease-in;

}

.imgcard{
    background-color: steelblue;
    width: 168px;
    height: 201px;
    margin: 0 12px;
    /* margin:0 auto ; */
}
img
{
    width: 100%;
    border-radius: 12px;
}

.cheading{
    margin-top: 150px;
  animation: slideInFromBottom 500ms ease-in;

}
.contactus_heading{
    text-align: center;
    margin: 21px auto;
}

.small_heading{
    margin-bottom: 25px;
    padding: 5px;
    text-align: center;
}

.email{
    text-align: center;
    margin-bottom: 25px;
}
.email a {
    color: grey;
}
.contactus{
    display: flex;
   margin-bottom: 35px;
   justify-content: center;
   margin-left: -76px;
}

.contactus a{
    color: black;
    margin: 0 40px;
}


@media (max-width: 900px){
    .aboutus_para{
        text-align: center;
        line-height: 1.3;
        padding: 23px;
        width: 500px;
    }
    
}

@media (max-width: 400px) {
  .aboutus {
    margin-top: 30px;
  }
  .aboutus_para {
    width: 100%;
  }
  .whoweare {
    margin: 0px 13px;
  }
  .imgcard {
    width: 195px;
    height: 270px;
    margin: 0;
  }
  img {
    height: 100%;
  }
}

</style>