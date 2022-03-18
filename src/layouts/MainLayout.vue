<template>
  <q-layout view="hHh lpR fff">
    <q-header elevated class="bg-primary text-white" height-hint="98">
      <q-toolbar class="text-white shadow-2 rounded-borders">
        <q-btn icon="home" to="/" flat label="Homepage" />
        <q-space />
        <q-tabs v-model="tab" shrink>
          <q-route-tab to="/blog" label="Blog" />
          <q-route-tab to="/contact" label="Contato" />
          <q-btn label="Login" color="secundary">
            <q-menu>
              <div class="q-pa-lg">
                <div class="text-h6 q-mb-md">Login</div>
                  <q-form @submit="onSubmit" class="q-gutter-md">
                    <q-input type="text" label="username" />
                    <q-input type="password" label="password" />
                    <div>
                      <q-btn label="submit" type="submit" color="primary" />
                    </div>
                  </q-form>
              </div>
            </q-menu>
          </q-btn>
        </q-tabs>
      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>

    <q-footer elevated class="bg-grey-8 text-white">
      <q-toolbar>
        <q-toolbar-title>Até mais, agradeço a visita !!</q-toolbar-title>
        <q-icon size="md" name="email" />
        <q-icon size="md" name="phone" />
        <q-icon size="md" name="location_on">
          <FormLogin />
        </q-icon>
      </q-toolbar>
    </q-footer>
  </q-layout>
</template>

<script>

import { defineComponent, ref } from "vue";

export default defineComponent({
  name: "MainLayout",
})
</script>
