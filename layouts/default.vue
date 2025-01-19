<template>
  <div class="min-h-screen flex flex-col">
    <!-- Hoofdinhoud -->
    <div class="animate-fade animate-once animate-delay-[500ms] flex-grow">
      <slot />
    </div>

    <!-- Footer -->
    <footer class="mt-10 mb-[2cm]">
      <hr class="my-3 border-gray-600" />
      <div class="text-center">
        <!-- Link naar contactpagina -->
        <h1 class="text-1.7xl font-bold">
          <a 
            href="http://localhost:3000/page/contact" 
            class="underline contact-link"
          >
            Contact Me
          </a>
        </h1>
        <p>Located in Brussels - Belgium</p>
        <p>
          E-mail: 
          <a href="mailto:alison.kremer@student.luca-arts.be" class="underline">
            alison.kremer@student.luca-arts.be
          </a>
        </p>
      </div>
    </footer>
  </div>
</template>

<style scoped>
footer {
  font-size: 0.775rem; /* Tekst kleiner maken */
  color: #4a5568; /* Grijstint */
}

.contact-link {
  text-decoration: underline;
  text-decoration-color: gray; /* Grijze lijn onder tekst */
  text-decoration-thickness: 2px;
}
.contact-link:hover {
  color: #2d3748; /* Donkerdere grijstint bij hover */
  text-decoration-color: #718096; /* Lichtere grijze lijn bij hover */
}
</style>
