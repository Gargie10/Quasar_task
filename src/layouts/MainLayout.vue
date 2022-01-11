<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated>
      <q-toolbar>
       

        <q-toolbar-title>
          Internship Task
        </q-toolbar-title>

        <div>By - {{name}}</div>
      </q-toolbar>
    </q-header>

   

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
export default {
  

data() {
  return {
    name : "Gargie Nimbalkar",
  }
}
};
</script>
