<template>
  <div class="banner">
    <div class="btitle">
      Manage your <br> time well
    </div>
    <div class="blogo">
      <i class="fa-regular fa-file"></i>
    </div>
  </div>
  <div class="categories">
     <h5>Categories</h5>
    <div class="types">
      <div id="categorie">
        <div>
          <span class="clogo"><i class="fa-solid fa-briefcase"></i></span>
        </div>
        <span class="ctitle">Work</span>
      </div>
      <div id="categorie">
        <div>
          <span class="plogo"><i class="fa-solid fa-user-large"></i></span>
        </div>
        <span class="ctitle">Personal</span>
      </div>
      <div id="categorie">
        <div>
          <span class="slogo"><i class="fa-solid fa-cart-shopping"></i></span>
        </div>
        <span class="ctitle">Shopping</span>
      </div>
      
        <div id="categorie">
            <div>
             <span class="hlogo"><i class="fa-solid fa-heart-pulse"></i></span>
            </div>
           <span class="ctitle">Health</span>
       </div>
    </div>
  </div>
  <div class="taskList">
    <h5>You have 5 tasks for today</h5>
    <div class="tasks">
     
          <div class="task">
            <div class="tInfo"><span class="number">01</span><span class="tTitle"> Daily challeng</span></div> 
            <div class="tButton">
              <button class="button1"><i class="fa-regular fa-pen-to-square"></i></button>
              <button class="button2"><i class="fa-solid fa-trash-can"></i></button>
            </div> 
          </div>
          <div class="task">
            <div class="tInfo"><span class="number">01</span><span class="tTitle"> Daily challeng</span></div> 
            <div class="tButton">
              <button class="button1"><i class="fa-regular fa-pen-to-square"></i></button>
              <button class="button2"><i class="fa-solid fa-trash-can"></i></button>
            </div> 
          </div>
          <div class="task">
            <div class="tInfo"><span class="number">01</span><span class="tTitle"> Daily challeng</span></div> 
            <div class="tButton">
              <button class="button1"><i class="fa-regular fa-pen-to-square"></i></button>
              <button class="button2"><i class="fa-solid fa-trash-can"></i></button>
            </div> 
          </div>
          <div class="task">
            <div class="tInfo"><span class="number">01</span><span class="tTitle"> Daily challeng</span></div> 
            <div class="tButton">
              <button class="button1"><i class="fa-regular fa-pen-to-square"></i></button>
              <button class="button2"><i class="fa-solid fa-trash-can"></i></button>
            </div> 
          </div>
          <div class="task">
            <div class="tInfo"><span class="number">01</span><span class="tTitle"> Daily challeng</span></div> 
            <div class="tButton">
              <button class="button1"><i class="fa-regular fa-pen-to-square"></i></button>
              <button class="button2"><i class="fa-solid fa-trash-can"></i></button>
            </div> 
          </div>
          <div class="task">
            <div class="tInfo"><span class="number">01</span><span class="tTitle"> Daily challeng</span></div> 
            <div class="tButton">
              <button class="button1"><i class="fa-regular fa-pen-to-square"></i></button>
              <button class="button2"><i class="fa-solid fa-trash-can"></i></button>
            </div> 
          </div>
      
      

    </div>
  </div>
  
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'IndexPage'
})
</script>
<style scoped>
.banner{
  background-image: linear-gradient(to right, #757dedb7, #4c4a4892);
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 4px 35px;
  margin: 20px 15px;
  border-radius: 15px;
}
.btitle{
  color: white;
  font-size: 16px;
}
.blogo{
  font-size: 54px;
  color: rgb(197, 200, 243);
}
h5{
  margin-left: 15px;
  font-size: 15px;
  font-weight: 900;
}
.types{
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  /* padding: 0px 30px; */
  /* border: 2px solid red; */
  /* gap: 10px; */
  /* justify-content: space-evenly; */
  /* justify-content: space-between; */
}
#categorie{
  display: grid;
  text-align: center;
  align-items: center;
  justify-content: center;
}
.clogo{
 font-size: 22px;
 border: 1px solid rgba(6, 28, 153, 0.53);
 padding: 10px 12px;
 border-radius: 12px;
 color: rgba(43, 137, 239, 0.737);
}
.plogo{
 font-size: 22px;
 border: 1px solid rgba(216, 219, 23, 0.865);
 padding: 10px 12px;
 border-radius: 12px;
 color: rgba(239, 161, 43, 0.621);
}
.slogo{
 font-size: 22px;
 border: 1px solid rgba(22, 182, 8, 0.737);
 padding: 10px 12px;
 border-radius: 12px;
 color: rgba(21, 200, 72, 0.546);
}
.hlogo{
 font-size: 22px;
 border: 1px solid rgba(246, 15, 15, 0.763);
 padding: 10px 12px;
 border-radius: 12px;
 color: rgba(237, 10, 10, 0.806);
}
.ctitle{
  text-align: center;
  margin-top: 20px;
  font-weight: 700;
  /* border: 2px solid skyblue; */
}
.task{
  /* border: 1px solid rgb(98, 89, 89); */
  box-shadow: 2px 1px 6px 1px rgb(159, 222, 226);
  margin: 22px 15px;
  padding: 12px 8px;
  border-radius: 10px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  
}
.tInfo{
  display: flex;
  justify-content: center;
  align-items: center;
}
.number{
  font-size: 18px;
  font-weight: 900;
  color: #636693b9;
}
.tTitle{
  font-weight: 900;
  margin-left: 20px;
  color: rgb(144, 136, 141);
}
.button1{
  border: none;
  background-color: white;
  font-size: 20px;
  color: rgb(111, 111, 218);
  margin-right: 13px;
  cursor: pointer;
}
.button2{
  border: none;
  background-color: white;
  font-size: 20px;
  color: rgb(237, 127, 127);
  margin-right: 10px;
  cursor: pointer;
}
</style>
