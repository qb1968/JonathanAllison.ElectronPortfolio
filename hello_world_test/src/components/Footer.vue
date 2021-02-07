<template>
  <div class="foot">
    <h2>Get in Touch</h2>
    <div class="links">
    <a href="https://github.com/qb1968"><i class="fa fa-github" style="font-size: 40px;"></i></a>
    <a href ="https://www.linkedin.com/in/jonathan-allison68/"><i class="fa fa-linkedin" style="font-size: 40px;"></i></a>
    <a href ="mailto:mark.allison75@gmail.com"><i class="fa fa-at" style="font-size: 40px;"></i></a>
    <a href="../resume.pdf" target="_blank" ><i class="fa fa-file" style="font-size: 40px;"/></a>
    </div>
    <p>Created By Jonathan Allison 2021</p>
  </div>
</template>

<script>
export default {
  name: 'Footer',
  props: {
    msg: String
  }
}
</script>

<style>
.foot {
  margin-top: 45px;
  background-color: rgb(1, 240, 240);
  height: 100px;
  
}
.con {
    font-size:24px;
}
a {
    color:black;
}
 .links {
     display: flex;
     justify-content: space-evenly;
     color:black;
     align-items: center;
 }
</style>