<template>
    <div>
        <div>
            <p class="headline">mtPAge</p>
            <v-breadcrumbs
            active-class="color"
            :items="items"
            class="pt-0 mt-n3 pl-0 main"
            large
            ></v-breadcrumbs>
        </div>

        <card1/>
        <card2/>
        <card3/>
        
    </div>
</template>
<script>
import card1 from "../components/analy/card1"
import card2 from "../components/analy/card2"
import card3 from "../components/analy/card3"
export default {
    data(){
        return{
            items: [
        {
          text: 'Dashboard',
          disabled: false,
          to: '/',
        },
        {
          text: 'Analytics',
          disabled: false,
          to: '/Analytics',
        },
      ],
        }
    },
    components:{
      card1,
      card2,
      card3,
      }
    
}
</script>

<style >
.main .v-breadcrumbs__item{
  color: grey!important;
}
.main .v-breadcrumbs__item--disabled{
  color:rgb(0, 47, 255)!important
}
    
</style>