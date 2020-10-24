<template lang="html">
  <div>
    <vs-tabs >
      <vs-tab label="Home">
        <div class="con-tab-ejemplo">
          Home
        </div>
      </vs-tab>
      <vs-tab :badge="10" :badgeStyle="{background:'#ff0000', color: '#fff'}" label="Service">
        <div class="con-tab-ejemplo">
          Service
        </div>
      </vs-tab>
      <vs-tab :badge="badgeNumber" label="Dynamic badge">
        <div class="con-tab-ejemplo">
          <button @click="incrNumber">Increase</button>
        </div>
      </vs-tab>
      <vs-tab disabled label="Disabled">
        <div class="con-tab-ejemplo">
          Disabled
        </div>
      </vs-tab>
      <vs-tab label="Lorem ipsum dolor sit amet">
        <div class="con-tab-ejemplo">
          Lorem ipsum dolor sit amet
        </div>
      </vs-tab>
    </vs-tabs>
  </div>
</template>

<script>
export default {
    data(){
        return {
            badgeNumber: 3
        }
    },
    methods:{
        incrNumber: function(){
            this.badgeNumber++;
        }
    }
}
</script>

<style lang="css">
</style>
