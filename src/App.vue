<script setup>
import AppCard from './components/AppCard.vue'
import AppTitle from './components/AppTitle.vue'
import FormStep from './components/FormStep.vue'
</script>

<template>
  <main class="h-screen overflow-hidden" id="main">
    <section role="grid" id="grid">
      <nav class="bg-[url('./src/assets/images/bg-sidebar-mobile.svg')] bg-no-repeat bg-cover">
        <div class="w-[50%] h-[50%] mx-auto flex items-center justify-center gap-4 md:flex-col">
          <form-step />
          <form-step />
        </div>
      </nav>
      <section class="w-[90%] mx-auto -mt-20 rounded-xl">
        <app-card>
          <app-title>Personal info</app-title>
          <p class="text-sm mt-4">Please provide your name, email address, and phone number.</p>
        </app-card>
      </section>
      <section class="bg-white">
        <div class="w-[90%] mx-auto flex items-center justify-between h-full">
          <button>Go Back</button>
          <button>Next Step</button>
        </div>
      </section>
    </section>
  </main>
</template>
