<template>
<q-page class="flex flex-center ">
  <div>
    <div class="row justify-center items-center">
    <div class="q-gutter-y-md" style="max-width: 600px">
        <q-tabs
          v-model="tab"
          dense
          class="q-ml-md bg-grey-3 text-grey-7"
          active-color="white"
          active-bg-color="info"
          color="grey-3"
          indicator-color="transparent"
          style="border-radius: 20px; width: 370px;"
          align="justify"
          narrow-indicator
        >
          <q-tab style="border-radius: 20px;"  name="super resolution" label="Super Resolution" />
          <q-tab style="border-radius: 20px;"  name="noise remover" label="Noise Remover" />
        </q-tabs>

        

        <q-tab-panels class="q-mt-xs" v-model="tab" animated>
          <q-tab-panel class="q-mt-xs" name="super resolution">
            <q-card inline style="width: 370px; height: 300px;" class=" bg-grey-5  my-card">
            </q-card>
            <div class="row q-mt-sm">
              <q-card flat style="width: 400px; max-height: 300px;" class="my-card text-body1">
              <q-card-section>
                {{text_one}}
              </q-card-section>
              <q-card-section >
                {{ text_two }}
              </q-card-section>
              </q-card>
            </div> 
          </q-tab-panel>

          <q-tab-panel class="q-mt-xs" name="noise remover">
            <q-card inline style="width: 370px; height: 300px;" class=" bg-grey-5  my-card">
    
            </q-card>
            <div class="row q-mt-sm">
              <q-card flat style="width: 400px; max-height: 300px;" class="my-card text-body1">
              <q-card-section>
                {{text_three}}
              </q-card-section>
              <q-card-section >
                {{ text_four}}
              </q-card-section>
              </q-card>
            </div> 
          </q-tab-panel>
        </q-tab-panels>
    </div>
  </div> 
  </div>
  </q-page>
</template>

<script>
import { ref } from 'vue'
export default {
  

data() {
  return {
   text_one: 'UpscalePics uses our state-of-the-art artificial intelligence to upscale and enhance images (also called super-resolution).',
   text_two : 'The Super Resolution uses machine learning to clarify, sharpen, and upscale the photo without losing its content and defining characteristics',
   
   text_three: 'UpscalePics uses our state-of-the-art artificial intelligence to upscale and enhance images (also called noise-remover).',
   text_four : 'The Noise Remover uses machine learning to clarify, sharpen, and upscale the photo without losing its content and defining characteristics',

   tab: ref('super resolution'),
    
  };
},

};
</script>

