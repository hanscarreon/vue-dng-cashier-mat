<template>
 
 <div class="page-container md-layout-column">
    <md-toolbar class="md-primary">
      <md-button class="md-icon-button" @click="showNavigation = true">
        <md-icon>menu</md-icon>
      </md-button>
      <span class="md-title">My Title</span>

     
    </md-toolbar>

    <md-drawer :md-active.sync="showNavigation" md-swipeable>
      <md-toolbar class="md-transparent" md-elevation="0">
        <span class="md-title">My App name</span>
      </md-toolbar>

      <md-list>
        <md-list-item>
          <md-icon>move_to_inbox</md-icon>
          <span class="md-list-item-text">Inbox</span>
        </md-list-item>

        <md-list-item>
          <md-icon>send</md-icon>
          <span class="md-list-item-text">Sent Mail</span>
        </md-list-item>

        <md-list-item>
          <md-icon>delete</md-icon>
          <span class="md-list-item-text">Trash</span>
        </md-list-item>

        <md-list-item>
          <md-icon>error</md-icon>
          <span class="md-list-item-text">Spam</span>
        </md-list-item>
      </md-list>
    </md-drawer>


    <md-content style=" min-height: 100vh;">
      <div class="md-layout">
        <div class="md-layout-item md-size-40 m-2">
          <ListCart/>
        </div>
         <div class="md-layout-item">
          
        </div>
      </div>
    </md-content>
  </div>
</template>

<script>
import ListCart from '../Pages/ListCart.vue'
  export default {
    name: 'MainLayout',
    components:{ListCart},
    data: () => ({
      showNavigation: false,
      showSidepanel: false
    })
  }
</script>

<style lang="scss" scoped>
 .mt-3{
   margin-top: 3em;
 }
 .mt-2{
   margin-top: 2em;
 }
.m-2{
   margin: 2em;
 }
 md-content{
   min-height: 100vh;
 }
  
  // .page-container {
  //   overflow: hidden;
  //   position: relative;
  //   border: 1px solid rgba(#000, .12);
  // }

  //  // Demo purposes only
  // .md-drawer {
  //   width: 230px;
  //   max-width: calc(100vw - 125px);
  // }

  // .md-content {
  //   padding: 16px;
  //   min-height: 100vh;

  // }
  .red{
    background: red;
  }
  .blue{
    background: blue;
  }
  .green{background: green;}
  .yellow{background: yellow;}
  .gray{background: gray;}
  .black{background: black;}
  
</style>