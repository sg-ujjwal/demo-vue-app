<template>
  <div class="home_body">
    <div class="container">
      <div class="row">
          <div class="item-4">
             <div class="item_wrap">
                <div class="header">
                  <h4>New Orders</h4>
                </div>
                  <CardBox/>
                  <CardBox/>
                  <CardBox/>
             </div>
          </div>
          <div class="item-4">
              <div class="item_wrap">
                <div class="header">
                  <h4>In Progress</h4>
                </div>
                <CardBox/>
                <CardBox/>
             </div>
          </div>
          <div class="item-4">
              <div class="item_wrap">
                <div class="header">
                  <h4>Waiting for buyer</h4>
                </div>
               <CardBox/>
             </div>
          </div>
          <div class="item-4">
              <div class="item_wrap">
                <div class="header">
                  <h4>Completed</h4>
                </div>
                <CardBox/>
                <CardBox/>
             </div>
          </div>
      </div>
  </div>
  </div>
</template>

<style lang="scss">
@import "@/assets/sass/home";
@import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap');

</style>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import CardBox from '@/components/card-item/card-box.vue'; // @ is an alias to /src


@Component({
  components: {
    CardBox,
  },
})
export default class Home extends Vue {

}
</script>