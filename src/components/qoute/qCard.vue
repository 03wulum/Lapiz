<template>
  <div class="card">
 <v-card
    class="mx-auto"
    color="#2962FF"
    dark
    max-width="400"
  >
      <v-card-actions>
      <v-list-item class="grow">
        <v-list-item-avatar color="grey darken-3">
          <v-img
            class="elevation-6"
            alt=""
            src="https://avataaars.io/?avatarStyle=Transparent&topType=ShortHairShortCurly&accessoriesType=Prescription02&hairColor=Black&facialHairType=Blank&clotheType=Hoodie&clotheColor=White&eyeType=Default&eyebrowType=DefaultNatural&mouthType=Default&skinColor=Light"
          ></v-img>
        </v-list-item-avatar>

      </v-list-item>
    </v-card-actions>
    
    <div class="parentQ" >
      <div class="qReply" style="width: 280px"> <v-list-item-title>Evan You</v-list-item-title>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
      </div>
    </div>

    <v-card-actions>
      <v-list-item class="grow">

        <v-row
          align="center"
          justify="end" class="icon-reactions"
        >
        <div>
          <v-icon class="mr-1">
            mdi-heart
          </v-icon>
          <span >256</span>   
        </div>
 
        <div>
                 <v-icon class="mr-1">
            mdi-share-variant
          </v-icon>

          <span class="subheading">45</span> 
        </div>
        <div>
              <v-icon class="mr-1" @click="$emit('toggleReply')">mdi-comment</v-icon>
                              <span class="subheading">45</span>
        </div>          
        </v-row>
      </v-list-item>
    </v-card-actions>
    <div v-if="isQreplyToggled">
       <v-col
        cols="12"
        md="12"
      >
        <v-textarea
          solo
          name="input-7-4"
          label="Solo textarea"
        ></v-textarea>
      </v-col>   
    </div>

    <div class="thread" >
        <v-list-item-avatar color="grey darken-3">
          <v-img
            class="elevation-6 profile-image"
            alt=""
            src="https://avataaars.io/?avatarStyle=Transparent&topType=ShortHairShortCurly&accessoriesType=Prescription02&hairColor=Black&facialHairType=Blank&clotheType=Hoodie&clotheColor=White&eyeType=Default&eyebrowType=DefaultNatural&mouthType=Default&skinColor=Light"
          ></v-img>
        </v-list-item-avatar>
      <div class="qReply" style="width: 200px">
                <v-list-item-content>
          <v-list-item-title>Evan You</v-list-item-title>
        </v-list-item-content>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
      </div>
    </div>
    <v-card-actions>
      <v-list-item class="grow">

        <v-row
          align="center"
          justify="end" class="icon-reactions"
        >
        <div>
          <v-icon class="mr-1">
            mdi-heart
          </v-icon>
          <span >256</span>   
        </div>
        <div>
                 <v-icon class="mr-1">
            mdi-share-variant
          </v-icon>

          <span class="subheading">45</span> 
        </div>
        <div>
              <v-icon class="mr-1" @click="$emit('toggleReply')">mdi-comment</v-icon>
                              <span class="subheading">45</span>
        </div>          
        </v-row>
      </v-list-item>
    </v-card-actions>
  </v-card>
</div>
</template>


<script lang="ts">
  import Vue from 'vue'

  export default Vue.extend({
    name: 'HelloWorld',

    props:  {
      isQreplyToggled: {
        required: false,
        type: Boolean,
        default: false
      }
    },


    methods: {
    }
  })
</script>

<style>
  .thread {
    border-left: 4px solid black;
    position:relative;
    margin-left: 40px;
    overflow: hidden;
    text-align: left
  }
  .profile-image {

  }
  .parentQ {
    position:relative;
    margin-left: 40px;
    overflow: hidden;
    text-align: left;
    margin-left: 1rem;
  }
  .qReply {
    margin-left: 15px; 
    margin-right: 10px;  
    padding-right: 2.5rem;
    word-break: break-word;
    white-space: normal;
    text-align: left;
  }
  .icon-reactions {
    display: flex;
    align-items: center;
    justify-content: space-evenly;
  }
</style>