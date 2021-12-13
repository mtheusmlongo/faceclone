<template>
  <q-layout view="lHh Lpr lFf">
    <q-header class="now items-center justify-between q-pt-sm">
     
      <q-img width="130px" class="q-mx-ms q-my-md" src= "../assets/facelogo.png" />
      
      <div>
        <q-icon
        class= "q-mx-sm q-pa-sm q-icon-custom"
        name= "fas fa-search"
        size= "25px"
        color= "black"
        />
        <q-icon
        class= "q-mx-sm q-pa-sm q-icon-custom"
        name=" fab fa-facebook-messenger"
        size= "25px"
        color= "black"
        /> 
       </div>
       <div class="flex flex-center full-whidth">
         <q-tabs v-model="tab" class="text-teal q-mx-sm full-width">
           <q-tab name="home" icon="fas fa-home" />
           <q-tab nome="users" icon="fas fa-users"/>
           <q-tab name="video" icon= "ondemand_video" />
           <q-tab name="store" icon="notifications" />
           <q-icon name="fas fa-bars" size="30px" class="q-mr-md q-icon-color" />
           
         </q-tabs>
       </div>


      </q-header>

   

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
export default {
name: 'MainLayout',
data () {
  return {
    tab : "home",
  };

 },
};

</script>

<style lang="scss" scoped>
.q-icon-custom {
background-color: #f2f2f2;
border-radius: 50%;
}
.q-tabs__content {
  height: 70px;
  width: 100%;
  display: flex;
  flex-direction: row;
  justify-content: space-around;
} 
.q-tab__icon {
  font-size: 20px;

}
.q-tab {
  padding:5px;
  }
  .q-tab--active{
    color: #1678f3
  }
  .q-tab--inactive{
     color:#656668
  }

</style>

