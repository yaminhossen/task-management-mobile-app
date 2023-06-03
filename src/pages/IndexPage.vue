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
.categories h5{
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
</style>
