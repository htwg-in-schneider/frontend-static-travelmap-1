<script setup lang="ts">
import globePng from '../assets/images/globe.png'
import globeHeroSvg from '../assets/images/globe-hero.svg'
import cloudSvg from '../assets/images/cloud.svg'
import pinSvg from '../assets/images/pin.svg'
import mapMyJourneyLogo from '../assets/images/mapMyJourneyLogo.svg'
</script>

<template>
  <!-- Navbar -->
  <nav class="fixed top-0 left-0 right-0 bg-white z-50 border-b border-gray-100">
    <input id="menu-toggle" type="checkbox" class="burger-checkbox" />
    <div class="max-w-6xl mx-auto md:px-0 px-6 py-4 flex items-center justify-between">
      <a href="#" class="flex items-center gap-2">
        <img :src="mapMyJourneyLogo" alt="MapMyJourney Logo" class="w-8 h-8" />
        <span class="font-bold text-gray-900">MapMyJourney</span>
      </a>
      <!-- Desktop Nav -->
      <div class="hidden md:flex gap-8 text-sm text-gray-600">
        <a href="#warum" class="hover:text-blue-500 transition-colors">Warum MapMyJourney</a>
        <a href="#features" class="hover:text-blue-500 transition-colors">Features</a>
        <a href="#so-funktionierts" class="hover:text-blue-500 transition-colors">So funktioniert's</a>
      </div>
      <!-- Burger Menu -->
      <label for="menu-toggle" class="md:hidden cursor-pointer" aria-label="Menü öffnen">
        <svg class="w-6 h-6 text-gray-700 burger-icon" fill="none" stroke="currentColor" viewBox="0 0 24 24">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
        </svg>
        <svg class="w-6 h-6 text-gray-700 close-icon" fill="none" stroke="currentColor" viewBox="0 0 24 24">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
        </svg>
      </label>
    </div>
    <!-- Mobile Nav -->
    <div class="mobile-menu border-t border-gray-100 bg-white px-6 py-4 flex-col gap-4 text-sm text-gray-600">
      <a href="#warum" class="hover:text-blue-500 transition-colors">Warum MapMyJourney</a>
      <a href="#features" class="hover:text-blue-500 transition-colors">Features</a>
      <a href="#so-funktionierts" class="hover:text-blue-500 transition-colors">So funktioniert's</a>
    </div>
  </nav>

  <!-- Hero -->
  <section class="min-h-screen flex items-center px-6 pt-20 md:pt-0">
    <div class="max-w-6xl mx-auto w-full flex flex-col md:flex-row items-center justify-between gap-12">
      <div class="flex-1">
        <h1 class="text-3xl md:text-4xl font-medium text-gray-900 leading-tight">
          Deine Reisen.<br />
          Dein Globus.<br />
          Deine Erinnerungen.
        </h1>
        <p class="mt-4 text-sm text-gray-500 max-w-md">
          Verknüpfe deine Reisefotos mit deinem virtuellen Globus und erlebe deine Abenteuer neu.
        </p>
        <a
          href="#warum"
          class="mt-6 inline-block bg-blue-500 text-white font-semibold px-6 py-3 rounded-2xl hover:bg-blue-700 transition-colors"
        >
          Leg los!
        </a>
      </div>
      <div class="flex-1 flex justify-center relative">
        <img :src="globePng" alt="Globus" class="w-72 md:w-96" />
      </div>
    </div>
  </section>

  <!-- Warum MapMyJourney -->
  <section id="warum" class="min-h-screen flex items-center px-6 bg-white">
    <div class="max-w-6xl mx-auto w-full">
      <h2 class="text-2xl md:text-3xl font-medium text-left text-gray-900 mb-16">
        Warum MapMyJourney?
      </h2>
      <div class="grid md:grid-cols-2 gap-16">
        <div>
          <h3 class="text-lg font-semibold text-gray-900 mb-4">
            1.000 Urlaubsfotos.<br />Und du schaust dir keins mehr an?
          </h3>
          <p class="text-sm text-gray-500 leading-relaxed">
            Nach dem Urlaub landen Hunderte Fotos in der Galerie, werden nie sortiert und geraten in Vergessenheit. Die schönsten Momente verschwinden zwischen Screenshots und Alltagsbildern.
          </p>
        </div>
        <div>
          <h3 class="text-lg font-semibold text-gray-900 mb-4">
            Gib deinen Erinnerungen einen Ort.
          </h3>
          <p class="text-sm text-gray-500 leading-relaxed">
            Jedes Foto bekommt seinen Platz auf deinem persönlichen 3D-Globus. So werden deine Reisen wieder lebendig.
          </p>
        </div>
      </div>
    </div>
  </section>

  <!-- Features -->
  <section id="features" class="min-h-screen flex items-center px-6">
    <div class="max-w-6xl mx-auto w-full">
      <h2 class="text-2xl md:text-3xl font-medium text-left text-gray-900 mb-16">Features</h2>
      <div class="grid md:grid-cols-3 gap-10">
        <!-- Feature 1 -->
        <div class="text-center border-3 border-blue-500 rounded-4xl p-8">
          <div class="w-16 h-16 mx-auto mb-4 flex items-center justify-center">
            <img :src="globeHeroSvg" alt="Globus" class="w-8 h-8" />
          </div>
          <h3 class="font-semibold text-gray-900 mb-2">Interaktiver 3D-Globus</h3>
          <p class="text-sm text-gray-500">
            Drehe, zoome und klicke dich durch deine Reiseziele. Jeder Marker erzählt eine Geschichte.
          </p>
        </div>
        <!-- Feature 2 -->
        <div class="text-center border-3 border-blue-500 rounded-4xl p-8">
          <div class="w-16 h-16 mx-auto mb-4 flex items-center justify-center">
            <img :src="cloudSvg" alt="Cloud" class="w-8 h-8" />
          </div>
          <h3 class="font-semibold text-gray-900 mb-2">Alles an einem Ort</h3>
          <p class="text-sm text-gray-500">
            Schluss mit Fotos auf fünf Geräten. Mit MapMyJourney sicher gespeichert und jederzeit abrufbar.
          </p>
        </div>
        <!-- Feature 3 -->
        <div class="text-center border-3 border-blue-500 rounded-4xl p-8">
          <div class="w-16 h-16 mx-auto mb-4 flex items-center justify-center">
            <img :src="pinSvg" alt="Pin" class="w-8 h-8" />
          </div>
          <h3 class="font-semibold text-gray-900 mb-2">Plane deine Reisen</h3>
          <p class="text-sm text-gray-500">
            Markiere deine Traumziele/Reiseziele und erstelle diese mit echten Erlebnissen.
          </p>
        </div>
      </div>
    </div>
  </section>

  <!-- So funktioniert's -->
  <section id="so-funktionierts" class="min-h-screen flex items-center px-6 bg-white">
    <div class="max-w-6xl mx-auto w-full flex flex-col md:flex-row items-center gap-16">
      <div class="flex-1">
        <h2 class="text-2xl md:text-3xl font-medium text-left text-gray-900 mb-12">So funktioniert's</h2>
        <div class="space-y-8">
          <div>
            <h3 class="font-semibold underline text-blue-500 mb-1">Schritt 1: Lade deine Fotos hoch</h3>
            <p class="text-sm text-gray-500">Einfach Bilder auswählen</p>
          </div>
          <div>
            <h3 class="font-semibold underline text-blue-500 mb-1">Schritt 2: Dein Globus füllt sich</h3>
            <p class="text-sm text-gray-500">Jedes Bild erscheint am Aufnahmeort auf deiner Weltkarte.</p>
          </div>
          <div>
            <h3 class="font-semibold underline text-blue-500 mb-1">Schritt 3: Erlebe und teile</h3>
            <p class="text-sm text-gray-500">Sammle Erinnerungen und lass dich zu neuen Reisen inspirieren.</p>
          </div>
        </div>
      </div>
      <div class="flex-1 flex justify-center">
        <img :src="mapMyJourneyLogo" alt="MapMyJourney Logo" class="w-64 md:w-80" />
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="bg-blue-500 py-8 text-center text-white text-sm">
    <div class="flex justify-center gap-6 mb-4">
      <a href="#warum" class="hover:underline">Warum MapMyJourney</a>
      <a href="#features" class="hover:underline">Features</a>
      <a href="#so-funktionierts" class="hover:underline">So funktioniert's</a>
    </div>
  </footer>
</template>

<style scoped>
.burger-checkbox {
  display: none;
}

.close-icon {
  display: none;
}

.mobile-menu {
  display: none;
}

.burger-checkbox:checked ~ .mobile-menu {
  display: flex;
}

.burger-checkbox:checked ~ div .burger-icon {
  display: none;
}

.burger-checkbox:checked ~ div .close-icon {
  display: block;
}

@media (min-width: 768px) {
  .mobile-menu {
    display: none !important;
  }
}
</style>
