<template>
  <!--
    <router-view />
-->
  <div class="q-pa-0">
    <q-layout
      view="lHh lpr lFf"
      container
      style="height: 100vh"
      class="shadow-2 rounded-borders"
    >
      <q-header elevated class="bg-brown-6">
        <q-toolbar>
          <q-avatar>
           <q-icon name="style" size="md"/>
          </q-avatar>
          <q-toolbar-title>Khipar - App</q-toolbar-title>
        </q-toolbar>
      </q-header>

      <q-footer elevated>
        <q-toolbar style="padding:0 !important">
            <div class="q-gutter-y-md" style="width:100vw">                 
              <q-card>
                <q-tab-panels v-model="tab" animated style="color:black !important;height: 80vh;">
                  <q-tab-panel name="mails" >
                    <div class="text-h6" >Mails</div>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                  </q-tab-panel>

                  <q-tab-panel name="alarms">
                    <div class="text-h6">Alarms</div>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                  </q-tab-panel>

                  <q-tab-panel name="movies">
                    <div class="text-h6">Movies</div>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                  </q-tab-panel>
                </q-tab-panels>

                <q-separator />

                <q-tabs
                  v-model="tab"
                  dense
                  class="bg-brown-6"
                  align="justify"
                  narrow-indicator
                  
                >
                  <q-tab name="mails" label="Bienvenida"><q-icon name="handshake" size="md"/></q-tab>
                  <q-tab name="alarms" label="Multimedia"><q-icon name="house" size="md"/> </q-tab>
                  <q-tab name="movies" label="Encuesta"><q-icon name="list" size="md"/></q-tab>
                </q-tabs>
              </q-card>
            </div>
        </q-toolbar>
      </q-footer>
    </q-layout>
  </div>
</template>

<script>
import { defineComponent } from "vue";
import { ref } from "vue";

export default defineComponent({
  name: "App",
  setup() {
    return {
      tab: ref("mails"),
    };
  },
});
</script>
