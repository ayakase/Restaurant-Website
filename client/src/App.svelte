<script lang="ts">
  import ThreeDPin from "./lib/components/custom/ThreeDPin.svelte";
</script>

<main
  class="bg-gradient-to-br from-orange-50 to-rose-100 text-gray-800 font-sans"
>
  <!-- Navbar -->
  <header
    class="fixed top-0 left-0 w-full z-50 bg-white/80 backdrop-blur-md shadow-sm"
  >
    <div class="max-w-7xl mx-auto px-6 py-4 flex items-center justify-between">
      <h1 class="text-2xl font-bold tracking-tight text-rose-600">
        La Palette
      </h1>
      <nav class="space-x-6 hidden md:flex">
        <a href="#hero" class="hover:text-rose-500 transition duration-300"
          >Home</a
        >
        <a href="#about" class="hover:text-rose-500 transition duration-300"
          >About</a
        >
        <a href="#menu" class="hover:text-rose-500 transition duration-300"
          >Menu</a
        >
        <a href="#gallery" class="hover:text-rose-500 transition duration-300"
          >Gallery</a
        >
        <a
          href="#testimonials"
          class="hover:text-rose-500 transition duration-300">Reviews</a
        >
        <a href="#contact" class="hover:text-rose-500 transition duration-300"
          >Contact</a
        >
      </nav>
    </div>
  </header>

  <!-- Hero Section -->
  <section
    id="hero"
    class="h-screen flex items-center justify-center relative overflow-hidden"
  >
    <img
      src="https://assets.epicurious.com/photos/624d9590857fa7e509238b59/16:9/w_1920,c_limit/RegionalChinese_HERO_033122_31320.jpg"
      alt="hero bg"
      class="absolute inset-0 w-full h-full object-cover opacity-80 animate-fadeIn"
    />
    <div class="relative z-10 text-center text-white max-w-2xl animate-fadeUp">
      <h2 class="text-5xl md:text-6xl font-bold drop-shadow-md">
        Taste the Art of Cuisine
      </h2>
      <p class="mt-4 text-xl md:text-2xl">An experience beyond dining</p>
      <a
        href="#reservation"
        class="inline-block mt-8 px-6 py-3 bg-rose-600 hover:bg-rose-700 text-white rounded-full shadow-lg transition"
        >Reserve a Table</a
      >
    </div>
  </section>
  <!-- <ThreeDPin></ThreeDPin> -->
  <!-- About Us -->
  <section
    id="about"
    class="py-24 px-6 md:px-20 lg:px-32 bg-white animate-fadeUp"
  >
    <div
      class="max-w-5xl mx-auto flex flex-col md:flex-row items-center gap-12"
    >
      <div class="md:w-1/2">
        <img
          src="https://images.unsplash.com/photo-1551218808-94e220e084d2"
          class="rounded-3xl shadow-lg"
          alt="About us"
        />
      </div>
      <div class="md:w-1/2 space-y-6">
        <h3 class="text-4xl font-semibold text-rose-600">Our Story</h3>
        <p class="text-lg leading-relaxed text-gray-700">
          La Palette was born from a dream to blend culinary craftsmanship with
          artistic ambiance. Our menu is a canvas, our chefs the artists, and
          every dish a masterpiece.
        </p>
        <p class="text-md text-gray-600">
          Located in the heart of the city, we bring the charm of fine French
          cuisine to a cozy, inviting space perfect for any occasion.
        </p>
      </div>
    </div>
  </section>

  <!-- Menu -->
  <section
    id="menu"
    class="py-24 px-6 md:px-20 lg:px-32 bg-gradient-to-b from-rose-100 to-orange-50 animate-fadeUp"
  >
    <div class="text-center mb-12">
      <h3 class="text-4xl font-semibold text-rose-600">Featured Menu</h3>
      <p class="text-gray-700">Explore our chef's seasonal picks</p>
    </div>
    <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-10">
      <!-- Menu Item -->
      <div
        class="bg-white rounded-3xl shadow-lg overflow-hidden transform hover:scale-105 transition duration-300"
      >
        <img
          src="https://images.unsplash.com/photo-1504674900247-0877df9cc836"
          alt="Dish 1"
          class="w-full h-56 object-cover"
        />
        <div class="p-6">
          <h4 class="text-2xl font-bold text-rose-600">Seared Duck Breast</h4>
          <p class="text-gray-600 mt-2">
            With honey-glazed carrots and cherry reduction
          </p>
          <div class="mt-4 text-right font-semibold text-gray-800">$28</div>
        </div>
      </div>
      <!-- Repeat more dishes similarly... -->
    </div>
  </section>

  <!-- Gallery -->
  <section
    id="gallery"
    class="py-24 px-6 md:px-20 lg:px-32 bg-white animate-fadeUp"
  >
    <div class="text-center mb-12">
      <h3 class="text-4xl font-semibold text-rose-600">Gallery</h3>
      <p class="text-gray-700">A glimpse of our cuisine and ambiance</p>
    </div>
    <div class="grid grid-cols-2 md:grid-cols-3 gap-6">
      {#each Array(10) as _, i}
        <img
          src="https://images.immediate.co.uk/production/volatile/sites/30/2020/08/chorizo-mozarella-gnocchi-bake-cropped-9ab73a3.jpg"
          alt="gallery"
          class="rounded-2xl hover:scale-105 transition duration-300"
        />
      {/each}

      <!-- more images... -->
    </div>
  </section>

  <!-- Testimonials -->
  <section
    id="testimonials"
    class="py-24 px-6 md:px-20 lg:px-32 bg-gradient-to-b from-orange-50 to-white animate-fadeUp"
  >
    <div class="text-center mb-12">
      <h3 class="text-4xl font-semibold text-rose-600">What Our Guests Say</h3>
    </div>
    <div class="grid md:grid-cols-2 gap-10">
      <div class="bg-white p-6 rounded-3xl shadow-lg">
        <p class="text-gray-700 italic">
          “Absolutely phenomenal! The flavors danced on my palate, and the
          ambiance was like stepping into a painting.”
        </p>
        <div class="mt-4 text-right font-bold text-rose-600">– Camille P.</div>
      </div>
      <div class="bg-white p-6 rounded-3xl shadow-lg">
        <p class="text-gray-700 italic">
          “The duck was divine and the desserts unforgettable. Can't wait to
          return!”
        </p>
        <div class="mt-4 text-right font-bold text-rose-600">– Jean-Luc R.</div>
      </div>
      <!-- more testimonials... -->
    </div>
  </section>

  <!-- Reservation Section -->
  <section
    id="reservation"
    class="py-24 px-6 md:px-20 lg:px-32 bg-white animate-fadeUp"
  >
    <div class="text-center mb-12">
      <h3 class="text-4xl font-semibold text-rose-600">Book a Table</h3>
      <p class="text-gray-700">Secure your seat for a memorable evening</p>
    </div>
    <form class="max-w-2xl mx-auto grid grid-cols-1 md:grid-cols-2 gap-6">
      <input
        type="text"
        placeholder="Name"
        class="p-4 rounded-lg border border-gray-300 focus:ring-2 focus:ring-rose-500"
      />
      <input
        type="email"
        placeholder="Email"
        class="p-4 rounded-lg border border-gray-300 focus:ring-2 focus:ring-rose-500"
      />
      <input
        type="tel"
        placeholder="Phone"
        class="p-4 rounded-lg border border-gray-300 focus:ring-2 focus:ring-rose-500"
      />
      <input
        type="date"
        class="p-4 rounded-lg border border-gray-300 focus:ring-2 focus:ring-rose-500"
      />
      <textarea
        placeholder="Special Requests"
        class="md:col-span-2 p-4 rounded-lg border border-gray-300 focus:ring-2 focus:ring-rose-500"
      ></textarea>
      <button
        type="submit"
        class="md:col-span-2 py-4 bg-rose-600 hover:bg-rose-700 text-white rounded-full shadow-md transition"
        >Submit</button
      >
    </form>
  </section>

  <!-- Contact Info -->
  <section
    id="contact"
    class="py-24 px-6 md:px-20 lg:px-32 bg-gradient-to-b from-white to-rose-100 animate-fadeUp"
  >
    <div class="text-center mb-12">
      <h3 class="text-4xl font-semibold text-rose-600">Visit Us</h3>
    </div>
    <div class="grid md:grid-cols-2 gap-12">
      <div></div>
      <div class="space-y-4 text-gray-700">
        <p><strong>Address:</strong> 123 Rue de Cuisine, Paris, France</p>
        <p><strong>Phone:</strong> +33 1 23 45 67 89</p>
        <p><strong>Opening Hours:</strong> Mon–Sun: 12PM – 10PM</p>
        <form class="mt-6">
          <label for="email" class="block mb-2 text-sm font-medium"
            >Subscribe to our newsletter</label
          >
          <div class="flex">
            <input
              id="email"
              type="email"
              placeholder="Your email"
              class="flex-grow p-3 rounded-l-lg border border-gray-300"
            />
            <button
              class="bg-rose-600 hover:bg-rose-700 text-white px-4 rounded-r-lg"
              >Subscribe</button
            >
          </div>
        </form>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="py-6 text-center text-sm text-gray-500 bg-white">
    &copy; 2025 La Palette. All rights reserved.
  </footer>
</main>

<style>
  @keyframes fadeIn {
    from {
      opacity: 0;
    }
    to {
      opacity: 1;
    }
  }
  @keyframes fadeUp {
    from {
      opacity: 0;
      transform: translateY(20px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }
  .animate-fadeIn {
    animation: fadeIn 2s ease-out both;
  }
  .animate-fadeUp {
    animation: fadeUp 1.5s ease-out both;
  }
</style>
