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
</style>
