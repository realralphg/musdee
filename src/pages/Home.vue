<template>
    <div>
        <div>
          <div class="bg-grey-3">
            <div class="text-center">
                <img src="images/divider.png" alt="" width="80%" >
            </div>
            <div class="text-center">
                <span class="ruban text-h4 text-weight-thin text-primary">Dorcas & Musa</span> <br>
                <span class="ruban text-h6 text-weight-light text-primary">#MusDee2020</span> <br>
                <span class="text-grey-7">We're getting married.</span>
            </div>
            <div class="text-center">
                <img src="images/divider.png" alt="" width="80%" >
            </div>   
          </div>
          <q-carousel
            v-model="slid"
            swipeable
            animated
            autoplay
            infinite
            control-color="secondary"
            :navigation="navigation"
            :navigation-position="navPos"
            height="400px"
            class="bg-grey-8 text-white"
            >

            <q-carousel-slide :name="carousel.name" class="q-pa-none" v-for="carousel in topCarousel" :key="carousel.id">
                <div>
                    <q-img :src="carousel.imageUrl" height="400px"/>
                    <div class="custom-caption absolute-bottom text-white text-h4 text-weight-light">
                    {{ carousel.title }}
                    </div>
                </div>
            </q-carousel-slide>
          </q-carousel>
        </div>

    <!-- Invitation C A R D -->
    <div class="row justify-center q-ma-md">
      <div class="text-center">
          <img src="images/divider.png" alt="" width="70%" >
      </div> 

      <q-card class="q-px-xl q-pt-xl text-white bg-grey-10 text-center" style="max-width: 350px">
        <span class="text-h4 text-weight-light text-primary align-center">Save The Date <br> </span>        
        <span class="text-h7 text-weight-light">TRADITIONALS <br> </span>
        <span class="text-h7 text-weight-thin">5th September, 2020 <br> <br> </span>        
        <span class="text-h7 text-weight-light">WEDDING CEREMONY <br> </span>
        <span class="text-h7 text-weight-thin">5th December, 2020 <br> <br> </span>        
        <span class="text-h7 text-weight-thin">Covenant Word Christian Center International, Jos. <br> <br> </span>
        <span class="text-h8">We are excited to celebrate with you! <br> </span> 
        <q-card-actions align="right">
          <a href="https://forms.gle/KaeAhx1qLRWivhtd9" target="_blank"><q-btn no-caps outline color="white" text-color="white" label="RSVP Now" /></a>          
        </q-card-actions>          
      </q-card>      
    </div>

    <div class="text-center">
        <img src="images/divider.png" alt="" width="70%" >
    </div>  

    <div class="text-h5 text-weight-light text-primary text-center">Wedding Colors <br> </div>        
    <div class="text-center">
      <q-chip clickable color="primary" text-color="white">
        Onion Purple
      </q-chip>
      <q-chip clickable color="secondary" text-color="white">
        Maroon
      </q-chip>
      <q-chip clickable color="primary" text-color="white" outline>
        White
      </q-chip>            
    </div>

    <div class="text-center">
        <img src="images/divider.png" alt="" width="70%" >
    </div> 

    <!-- Couple Toast-->
    <!-- Two Cards - Female-->
    <div class="row items-start justify-center  q-pa-md bg-grey-4 ">
      <q-card class="bg-primary" style="max-width: 300px">
          <img src="images/pic1.jpg" alt="">
      </q-card>

      <q-card class="q-pa-md text-grey-7 bg-grey-3" style="max-width: 300px; width: 100%"> 
          <span class="text-weight-light text-h5 text-black">Dee, baby</span>
          <p>May all sweethearts become couples <br>
              And may all couples remain sweethearts <br>
              May you all live as long as you like <br>
              And have all you like for as long as you live <br>
              The woman I truly love will never grow old to me.</p>                
      </q-card>
    </div>

    <!-- Two Cards - Male-->
    <div class="row items-start justify-center  q-pa-md bg-grey-4 ">
      <q-card class="q-pa-md text-grey-7 bg-grey-3" style="max-width: 300px; width: 100%"> 
          <span class="text-weight-light text-h5 text-black">Musa, love</span>
          <p>Because I love you truly <br>
              Because you love me, too <br>
              My very greatest happiness <br>
              Is sharing life with you <br> </p>                
      </q-card>

      <q-card class="bg-primary" style="max-width: 300px">
          <img src="images/pic3.jpg" alt="">
      </q-card>      
    </div> 

    <div class="bg-grey-8">
        <div class="text-center">
          <img src="images/divider.png" alt="" width="80%" >
        </div>          
        <div class="text-weight-light text-h4 text-white text-center">
          Our Love Story
        </div>
        <div class="text-center">
          <img src="images/divider.png" alt="" width="80%" >
        </div>
<!-- C H A T Love Story -->
        <div class="q-pr-md q-pl-md q-pb-md row justify-center">
            <div class="text-white" style="width: 100%; max-width: 500px">
              <q-chat-message
                label="Saturday, 19th"
              />

              <q-chat-message
                name="Dorcas"
                avatar="images/dee.jpg"
                :text="['We met online in 2012.']"
                sent
                stamp="15 minutes ago"
              />
              <q-chat-message
                name="Musa"
                avatar="images/musa.jpg"
                :text="['We met few weeks after and found out our parents knew each other for decades even before we were born']"
                stamp="14 minutes ago"
              />
              <q-chat-message
                name="Dorcas"
                avatar="images/dee.jpg"
                :text="['Our relationship grew from there, and although we had our mishaps our greatest bond has always been love and family.']"
                sent
                stamp="12 minutes ago"
              />
              <q-chat-message
                name="Musa"
                avatar="images/musa.jpg"
                :text="['Here we are now! Taking everything to the next and final level.']"
                stamp="11 minutes ago"
              /> 
                                      
            </div>
          </div>                
    </div>

<!-- Pre-Wedding Photos -->
    <div class="bg-grey-8">
        <div class="text-center">
          <img src="images/divider.png" alt="" width="80%" >
        </div>          
        <div class="text-weight-light text-h4 text-white text-center">
          Pre-wedding Photos
        </div>
        <div class="text-center q-mb-none q-pb-none">
          <img src="images/divider.png" alt="" width="80%" >
        </div>

        <q-page-container class="q-mx-xl text-center">  
          <div class="">
            <div class="q-pb-md">
                <q-img  class="radius" src="images/pic6.jpg" :ratio="4/3" />
            </div>

            <div class="q-pb-md">
                <q-img class="radius"  src="images/pic7.jpg" :ratio="4/3" />
            </div>

            <div class="q-pb-md">
                <q-img class="radius"  src="images/pic8.jpg" :ratio="4/3" />
            </div>

            <div class="q-pb-md">
                <q-img class="radius"  src="images/pic9.jpg" :ratio="4/3" />
            </div>

            <div class="q-pb-md">
                <q-img class="radius"  src="images/pic10.jpg" :ratio="4/3" />
            </div>

            <div class="q-pb-md">
                <q-img class="radius"  src="images/pic5.jpg" :ratio="4/3" />
            </div>    

            <div class="q-pb-md">
                <q-img class="radius"  src="images/pic2.jpg" :ratio="4/3" />
            </div> 
          </div>        
        </q-page-container>


        <div class="text-center">
          <img src="images/divider.png" alt="" width="80%" >
        </div>          
    </div>

<!-- Gift Registry -->
    <div class="bg-grey-4">
        <div class="text-center">
          <img src="images/divider.png" alt="" width="80%" >
        </div>          
        <div class="text-weight-light text-h4 text-grey-8 text-center">
          Gift Registry
        </div>
        <div class="text-center">
          <img src="images/divider.png" alt="" width="80%" >
        </div>

        <div class="text-grey-9 text-center q-mb-sm q-px-md">
          We are grateful in advance for all the pleasant gifts you have planned 
          to gift us with. You may wish to gift any of the items below or gift cash. 
          Again, thank you very plenty.
        </div>         
<!-- Gift Cards -->
        <div class="row justify-center q-gutter-md">
          <q-card class="bg-grey-3" style="width: 100%; max-width: 300px;">
            <img src="images/cash.jpg">
            <q-card-section>
              <div class="text-grey-8">
                Cash Gift
              </div>              
            </q-card-section>
            <q-card-actions align="right">
              <a href="https://paystack.com/pay/6jkudidv7e" target="_blank"><q-btn no-caps glossy rounded color="primary" icon="favorite" label="Gift This" /></a>
            </q-card-actions>
          </q-card>

          <q-card class="bg-grey-3" style="width: 100%; max-width: 300px;">
            <img src="images/microwave.jpg">
            <q-card-section>
              <div class="text-grey-8">
                #50,000 - Hisense Microwave
              </div>              
            </q-card-section>
            <q-card-actions align="right">
              <a href="https://paystack.com/pay/6jkudidv7e" target="_blank"><q-btn no-caps glossy rounded color="primary" icon="favorite" label="Gift This" /></a>
            </q-card-actions>
          </q-card>  

          <q-card class="bg-grey-3" style="width: 100%; max-width: 300px;">
            <img src="images/gascooker.png">
            <q-card-section>
              <div class="text-grey-8">
                #130,000 - Gascooker
              </div>              
            </q-card-section>
            <q-card-actions align="right">
              <a href="https://paystack.com/pay/6jkudidv7e" target="_blank"><q-btn no-caps glossy rounded color="primary" icon="favorite" label="Gift This" /></a>
            </q-card-actions>
          </q-card>  

          <q-card class="bg-grey-3" style="width: 100%; max-width: 300px;">
            <img src="images/washing.jpg">
            <q-card-section>
              <div class="text-grey-8">
                #100,000 - Washing Machine
              </div>              
            </q-card-section>
            <q-card-actions align="right">
              <a href="https://paystack.com/pay/6jkudidv7e" target="_blank"><q-btn no-caps glossy rounded color="primary" icon="favorite" label="Gift This" /></a>
            </q-card-actions>
          </q-card>                      
        </div>

<!-- Appreciation -->
        <div class="text-center q-pa-md">
          Thank's for your love <br>
          We are excited to celebrate with you! <br>  
          Watch this space for our post-wedding Photo Gallery!       
        </div>

        <div class="text-center">
          <img src="images/divider.png" alt="" width="80%" >
        </div>          

<!-- Floating Button -->
      <q-page-sticky position="bottom-right" :offset="[18, 18]">
        <q-fab
          v-model="fabRight"
          autoplay
          animated
          transition-prev="slide-right"
          transition-next="slide-left"    
          swipeable
          vertical-actions-align="right"
          color="primary"
          glossy
          icon="add"
          direction="up"
        >
          <q-fab-action label-position="left" color="primary" to="/giftregistry" icon="card_giftcard" label="Gift Registry" />
          <q-fab-action label-position="left" color="primary" @click="contactus=true" icon="phone" label="Contact Us" />
        </q-fab>  
      </q-page-sticky> 

    <!-- Dialogs -->
    <q-dialog v-model="contactus">
      <ContactUs/>
    </q-dialog> 

    </div>  
  </div>
</template>

<script>
import ContactUs from '../components/Dialogs/ContactUs'

export default {

    components:{
    ContactUs
  },

  data () {
    return {    
      fabRight: false,
      contactus: false,
    // for Carousel
      slid: 'moonlove',
      navigation: true,
      navPos: 'bottom',
      slide: 1,

      topCarousel: [
        {
          id: '1',
          name: 'moonlove',
          imageUrl: '/images/pic6.jpg',
          title: '05th December, 2020',
        },
        {
          id: '2',
          name: 'lovecircle',
          imageUrl: '/images/pic7.jpg',
          title: '#MusDee2020',
        },
        {
          id: '3',
          name: 'lovelove',
          imageUrl: '/images/pic8.jpg',
          title: '#Soulmates',
        },
        {
          id: '4',
          name: 'loveRing',
          imageUrl: '/images/pic9.jpg',
          title: '#Forever',
        },                         
      ],      
    }
  }

}
</script>

<style scoped>

.custom-caption{
    bottom: 50px;
    text-align: center;
    padding: 12px;
    background-color: rgba(0, 0, 0, .3);
}

.radius{
  border-radius: 15px 0px 15px 0px;
  max-width: 350px;
}


/* .ruban{
    font-family:'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
} */
</style>
