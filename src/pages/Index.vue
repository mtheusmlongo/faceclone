    <template>
      <q-page class= "q-nt-sm">
        <div class ="row q-pa-sm full-width">
          <q-avatar class= "q-mr-sm">
            <img src="https://cdn.quasar.dev/img/avatar.png" alt="" />
          </q-avatar>
          <q-input 
          rounded
          outlined 
          v-model="text" 
          label="No que você está pensando" 
          label-color="black" 
          >

            </q-input>
          </div>

          <div class="line q-mt-md" />
          <div class="row justify-around full-width q-pa-sm">
            <div>
              <q-icon
              color="red"
              name="fas fa-video"
              size="18px"
              class="q-mr-sm q-icon-color"
              >
              </q-icon>
              <label>Ao Vivo</label>
            </div>
              <div class="vertical-line"> </div>
              <div>
                <q-icon
                color="light-green-7"
                name="far-fa-images"
                size="20px"
                class="q-mr-sm q-icon-color"
                >
                </q-icon>
                
                <label>F</label>
                  <div class="vertical-line">
                    
                  </div>
              </div>  
            
            <div>
              <q-icon
              color="purple"
              name="meeting_room"
              size="18px"
              class="q-mr-sm q-icon-color"
              >
              </q-icon>
              <label>Salas</label>
            </div>
          </div>
              <div class="vertical-line"></div>
          
            
          <div class="line-strong q-mt-md"></div>
          
          <q-scroll-area horizontal class="container-new-room full-whidth">
          
            <div   
            class="row items-center justify-between q-px-md q-py-sm no-wrap full-width conta"
            >
            <div class="rounded-burron row text-center q-mr-md">
              <div class ="row items-center justify-center">
                <q-icon
                name="fas fa-video"
                color="purple"
                size="28px"
                class="q-mr-sm q-icon-color"
                >
                </q-icon>
                
              </div>
            </div>
            </div>
          </q-scroll-area>
            
          
      
      
      </q-page>
      

        
        </template>    

    <script>
    export default {
        name: "PageIndex",
        data() {
          return {
            text :"",

          };
        },
      };
    </script>



    <style lang="scss" scoped>
           
    .q-field {
      width: 82%;
    }
    .q-field control {
        height: 45px;
      }
    .conteiner-new-room{
      background-color: #fff; 
    }
    .conteiner-button {
      border:1px solid #cbed3c

    }
    .conteiner-new-room{
      height: 70px;
    }
    .conteiner-room {
      background-color:#fff ;
    }
    .rounded-button {
      border:1px solid #cbced3 ;
      border-radius: 27px ;
      padding: 4px 10px;

      div:first-child {
        width: 50%;
      }
      div{
        width: 50%;
      }
      label {
        color: #161616;
      }

      

    }
    </style>
