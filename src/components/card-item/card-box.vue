<template>
 <div class="item_box">
    <div class="item_body">
        <div class="del_toggle">
            <!-- <button @click="onClick">Click!</button> -->
            <div class="toggle_img" @click="onClick">
                <img src="../../assets/images/menu.png" alt="">
            </div>
            <div class="delet_btn" v-bind:class="{active: isActive}">
                <a href="#"><img src="../../assets/images/delete.png" alt="">Delete</a>
            </div>


        </div>
        <div class="media">
            <div class="media_img">
                <img src="../../assets/images/shoes.jpg" alt="">
            </div>
            <div class="media-body">
            <div class="media_content">
                <div class="product_action">
                    <span>In progress</span>
                </div>
                <div class="product_time">
                    <span> <img src="../../assets/images/clock.png" alt=""> Due in 2days, 5hrs</span>
                </div>
                <div class="hour_price">
                    <ul>
                    <li>5 hrs</li>
                    <li><b>$546</b></li>
                    </ul>
                </div>
            </div>
            </div>
        </div>
        <div class="checkbox">
            <label>
            <input type="checkbox" name="checkbox" value="css" checked />
            <span><del>Reply to John's message</del></span>
            </label>
            <label>
            <input type="checkbox" name="checkbox" value="js" />
            <span>Send a draft</span>
            </label>
        </div>
    </div>
    <div class="item_footer">
        <div class="footer_content">
        <div class="footer_left">
            <h5>View Order</h5>
        </div>
        <div class="footer_right">
            <div class="progress">
                <div class="bar" style="width:56%">
                </div>
            </div>
            <div class="chat_box">
                <img alt="" src="../../assets/images/chat.png">
            </div>
            <div class="profile_img">
            <img src="../../assets/images/profile.jpg" alt="">
            </div>
        </div>
        </div>
    </div>
</div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';


@Component
export default class CardBox extends Vue {
    public isActive: boolean = false;
 public onClick(): void {
    this.isActive = !this.isActive;
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
