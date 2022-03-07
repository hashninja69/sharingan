<template>
  <div class="megacontainer flex">
    <h1>First Semester</h1>
    <div class="master flex">
      <div class="col flex">
        <h3>Notes</h3>
        <ul id="hover" class="flex">
          <li><a href="#">C Programming</a></li>
          <li><a href="#">Office Automation</a></li>
          <li><a href="#">Computer Fundamentals</a></li>
        </ul>
      </div>
      <div class="col flex">
        <h3>Practical Files</h3>
        <ul  id="hover" class="flex">
          <li><a href="#">C Programming</a></li>
          <li><a href="#">Office Automation</a></li>
          <li><a href="#">Computer Fundamentals</a></li>
        </ul>
      </div>
      <div class="col flex">
        <h3>Question Papers</h3>
        <ul  id="hover" class="flex">
          <li><a href="#">C Programming</a></li>
          <li><a href="#">Office Automation</a></li>
          <li><a href="#">Computer Fundamentals</a></li>
        </ul>
      </div>
    </div>
  </div>
</template>




<script>
export default{
    data() {
        return {
            hover:'hoverr'
        }

    },
    methods:{
        run(){

        }
    }
}
</script>

<style >

.col a:hover{
    color: darkred;
    color: rebeccapurple;
    border-bottom: 1px solid white;

}
.megacontainer {
  background: url("./semback.png");
  height: 580px;
  filter: hue-rotate(45deg);
  align-content: center;
  flex-direction: column;
  text-align: center;
  z-index: 2;
  position: relative;
}

.megacontainer h1 {
  margin-top: 117px;
  margin-bottom: 12px;
  animation: slideInFromLeft 300ms ease-in;
  font-weight: 700;
}

.master {
  justify-content: space-evenly;
  height: 400px;
  width: 1018px;
  margin: 0 auto;
}

.col {
  height: 315px;
  width: 300px;
  background-color: transparent;
  border-radius: 12px;
  flex-direction: column;
  justify-content: center;
box-shadow: 0px 0px 13px 3px #191919;

  animation: slideInFromRight 300ms ease-in;
}

.col h3 {
  color: #fff;
}

.col ul {
  flex-direction: column;
}

.col li {
  margin: 12px 0;
}

.col a {
  color: #fff;
  font-size: 20px;
}





@media (max-width: 900px) {
  .megacontainer {
    height: 908px;
    flex-direction: column;
  }
  .megacontainer h1 {
    animation: slideInFromTop 300ms ease-in;
    margin-top: 25px;
    margin-bottom: -44px;
  }

  .col {
    background-color: #fff;
    animation: slideInFromBottom 300ms ease-in;
  }
  .col h3 {
    color: black;
  }

  .col a {
    color: black;
  }

  .container {
    height: 1272px;
    background-repeat: round;
  }
  .master {
    align-items: center;
    flex-direction: column;
    margin-top: 220px;
    width: auto;
  }

  .col {
    margin: 22px 0;
  }
}
</style>