<script lang="ts">
  import ThreeDPin from "./lib/components/custom/ThreeDPin.svelte";
  import TopNavBar from "./lib/components/general/TopNavBar.svelte";
</script>

<main>
  <!-- Navigation -->
  <TopNavBar></TopNavBar>

  <!-- Hero Section -->
  <section
    id="home"
    class="h-screen bg-gray-900 flex items-center relative overflow-hidden"
    style="background-image: url('https://placehold.co/1920x1080'); background-size: cover; background-position: center;"
  >
    <div class="absolute inset-0 bg-black bg-opacity-60"></div>
    <div class="container mx-auto px-4 z-10 text-center">
      <h1 class="text-4xl md:text-6xl font-bold text-white mb-4">
        <span class="text-yellow-500">Dimsum</span>
      </h1>
      <p class="text-xl md:text-2xl text-gray-200 mb-8">
        Authentic Taiwanese Dimsum Experience
      </p>
      <a
        href="#menu"
        class="bg-red-800 hover:bg-red-700 text-white px-8 py-3 rounded-full font-medium inline-block transition duration-300 mr-4"
        >View Menu</a
      >
      <a
        href="#contact"
        class="bg-transparent hover:bg-yellow-600 text-yellow-500 hover:text-white border border-yellow-500 hover:border-transparent px-8 py-3 rounded-full font-medium inline-block transition duration-300"
        >Make Reservation</a
      >
    </div>
  </section>

  <!-- About Section -->
  <section id="about" class="py-20 bg-white">
    <div class="container mx-auto px-4">
      <div class="text-center mb-12">
        <h2 class="text-3xl md:text-4xl font-bold mb-2">
          Our <span class="text-red-800">Story</span>
        </h2>
        <div class="w-24 h-1 bg-yellow-500 mx-auto"></div>
      </div>
      <div class="flex flex-col md:flex-row items-center">
        <div class="md:w-1/2 mb-8 md:mb-0 md:pr-8">
          <div class="rounded-lg overflow-hidden shadow-xl">
            <img
              src="https://placehold.co/600x400"
              alt="Restaurant Interior"
              class="w-full h-auto"
            />
          </div>
        </div>
        <div class="md:w-1/2">
          <h3 class="text-2xl font-semibold mb-4 text-red-800">
            Authentic Taiwanese Cuisine
          </h3>
          <p class="text-gray-700 mb-4">
            Hao Chi Dimsum proudly brings the authentic taste of Taiwan to
            Vietnam. As the first dimsum brand in Vietnam that combines
            traditional dimsum with Taiwanese milk tea, we offer a unique
            culinary experience.
          </p>
          <p class="text-gray-700 mb-6">
            Founded in 2015, our chefs have mastered the art of crafting
            delicate dimsum that balances texture and flavor. Each dish is
            handmade with carefully selected ingredients to ensure the highest
            quality.
          </p>
          <div class="flex flex-wrap">
            <div class="w-1/2 md:w-1/3 mb-4">
              <div class="flex items-center">
                <i class="fas fa-utensils text-yellow-600 mr-2"></i>
                <span>Fresh Ingredients</span>
              </div>
            </div>
            <div class="w-1/2 md:w-1/3 mb-4">
              <div class="flex items-center">
                <i class="fas fa-award text-yellow-600 mr-2"></i>
                <span>Award Winning</span>
              </div>
            </div>
            <div class="w-1/2 md:w-1/3 mb-4">
              <div class="flex items-center">
                <i class="fas fa-users text-yellow-600 mr-2"></i>
                <span>Family Friendly</span>
              </div>
            </div>
            <div class="w-1/2 md:w-1/3 mb-4">
              <div class="flex items-center">
                <i class="fas fa-leaf text-yellow-600 mr-2"></i>
                <span>Vegetarian Options</span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Menu Section -->
  <section id="menu" class="py-20 bg-gray-100">
    <div class="container mx-auto px-4">
      <div class="text-center mb-12">
        <h2 class="text-3xl md:text-4xl font-bold mb-2">
          Our <span class="text-red-800">Menu</span>
        </h2>
        <div class="w-24 h-1 bg-yellow-500 mx-auto mb-6"></div>
        <p class="text-gray-600 max-w-2xl mx-auto">
          Explore our extensive selection of handcrafted dimsum and specialty
          Taiwanese tea drinks.
        </p>
      </div>

      <!-- Menu Categories -->
      <div class="mb-12">
        <div class="flex flex-wrap justify-center space-x-2 md:space-x-4 mb-8">
          <button class="bg-red-800 text-white px-6 py-2 rounded-full mb-2"
            >All</button
          >
          <button
            class="bg-gray-200 hover:bg-red-800 hover:text-white px-6 py-2 rounded-full mb-2 transition duration-300"
            >Steamed Dimsum</button
          >
          <button
            class="bg-gray-200 hover:bg-red-800 hover:text-white px-6 py-2 rounded-full mb-2 transition duration-300"
            >Fried Dimsum</button
          >
          <button
            class="bg-gray-200 hover:bg-red-800 hover:text-white px-6 py-2 rounded-full mb-2 transition duration-300"
            >Buns</button
          >
          <button
            class="bg-gray-200 hover:bg-red-800 hover:text-white px-6 py-2 rounded-full mb-2 transition duration-300"
            >Milk Tea</button
          >
        </div>
      </div>

      <!-- Menu Items -->
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
        <!-- Menu Item 1 -->
        <div
          class="bg-white rounded-lg overflow-hidden shadow-md hover:shadow-xl transition duration-300"
        >
          <img
            src="https://placehold.co/400x300"
            alt="Har Gow"
            class="w-full h-48 object-cover"
          />
          <div class="p-6">
            <div class="flex justify-between items-center mb-2">
              <h3 class="text-xl font-bold text-gray-800">Har Gow</h3>
              <span class="text-yellow-600 font-bold">$6.50</span>
            </div>
            <p class="text-gray-600 text-sm mb-4">
              Delicate steamed crystal shrimp dumplings
            </p>
            <div class="flex justify-between items-center">
              <span
                class="inline-block bg-red-100 text-red-800 text-xs px-2 py-1 rounded-full"
                >Bestseller</span
              >
              <!-- <button
                class="text-red-800 hover:text-yellow-600 transition duration-300"
              >
                <i class="fas fa-plus-circle text-xl"></i>
                
              </button> -->
            </div>
          </div>
        </div>

        <!-- Menu Item 2 -->
        <div
          class="bg-white rounded-lg overflow-hidden shadow-md hover:shadow-xl transition duration-300"
        >
          <img
            src="https://placehold.co/400x300"
            alt="Siu Mai"
            class="w-full h-48 object-cover"
          />
          <div class="p-6">
            <div class="flex justify-between items-center mb-2">
              <h3 class="text-xl font-bold text-gray-800">Siu Mai</h3>
              <span class="text-yellow-600 font-bold">$5.80</span>
            </div>
            <p class="text-gray-600 text-sm mb-4">
              Open-faced dumplings with pork and shrimp
            </p>
            <div class="flex justify-between items-center">
              <span
                class="inline-block bg-red-100 text-red-800 text-xs px-2 py-1 rounded-full"
                >Popular</span
              >
              <!-- <button
                class="text-red-800 hover:text-yellow-600 transition duration-300"
              >
                <i class="fas fa-plus-circle text-xl"></i>
              </button> -->
            </div>
          </div>
        </div>

        <!-- Menu Item 3 -->
        <div
          class="bg-white rounded-lg overflow-hidden shadow-md hover:shadow-xl transition duration-300"
        >
          <img
            src="https://placehold.co/400x300"
            alt="BBQ Pork Bun"
            class="w-full h-48 object-cover"
          />
          <div class="p-6">
            <div class="flex justify-between items-center mb-2">
              <h3 class="text-xl font-bold text-gray-800">BBQ Pork Bun</h3>
              <span class="text-yellow-600 font-bold">$4.90</span>
            </div>
            <p class="text-gray-600 text-sm mb-4">
              Fluffy steamed buns with BBQ pork filling
            </p>
            <div class="flex justify-between items-center">
              <span
                class="inline-block bg-red-100 text-red-800 text-xs px-2 py-1 rounded-full"
                >Must Try</span
              >
              <!-- <button
                class="text-red-800 hover:text-yellow-600 transition duration-300"
              >
                <i class="fas fa-plus-circle text-xl"></i>
              </button> -->
            </div>
          </div>
        </div>

        <!-- Menu Item 4 -->
        <div
          class="bg-white rounded-lg overflow-hidden shadow-md hover:shadow-xl transition duration-300"
        >
          <img
            src="https://placehold.co/400x300"
            alt="Taro Milk Tea"
            class="w-full h-48 object-cover"
          />
          <div class="p-6">
            <div class="flex justify-between items-center mb-2">
              <h3 class="text-xl font-bold text-gray-800">Taro Milk Tea</h3>
              <span class="text-yellow-600 font-bold">$3.50</span>
            </div>
            <p class="text-gray-600 text-sm mb-4">
              Creamy taro-flavored milk tea with boba pearls
            </p>
            <div class="flex justify-between items-center">
              <span
                class="inline-block bg-red-100 text-red-800 text-xs px-2 py-1 rounded-full"
                >New</span
              >
              <!-- <button
                class="text-red-800 hover:text-yellow-600 transition duration-300"
              >
                <i class="fas fa-plus-circle text-xl"></i>
              </button> -->
            </div>
          </div>
        </div>

        <!-- Menu Item 5 -->
        <div
          class="bg-white rounded-lg overflow-hidden shadow-md hover:shadow-xl transition duration-300"
        >
          <img
            src="https://placehold.co/400x300"
            alt="Spring Rolls"
            class="w-full h-48 object-cover"
          />
          <div class="p-6">
            <div class="flex justify-between items-center mb-2">
              <h3 class="text-xl font-bold text-gray-800">Spring Rolls</h3>
              <span class="text-yellow-600 font-bold">$5.20</span>
            </div>
            <p class="text-gray-600 text-sm mb-4">
              Crispy fried rolls with vegetables and meat
            </p>
            <div class="flex justify-between items-center">
              <span
                class="inline-block bg-gray-100 text-gray-800 text-xs px-2 py-1 rounded-full"
                >Vegetarian Available</span
              >
              <!-- <button
                class="text-red-800 hover:text-yellow-600 transition duration-300"
              >
                <i class="fas fa-plus-circle text-xl"></i>
              </button> -->
            </div>
          </div>
        </div>

        <!-- Menu Item 6 -->
        <div
          class="bg-white rounded-lg overflow-hidden shadow-md hover:shadow-xl transition duration-300"
        >
          <img
            src="https://placehold.co/400x300"
            alt="Mango Pudding"
            class="w-full h-48 object-cover"
          />
          <div class="p-6">
            <div class="flex justify-between items-center mb-2">
              <h3 class="text-xl font-bold text-gray-800">Mango Pudding</h3>
              <span class="text-yellow-600 font-bold">$4.00</span>
            </div>
            <p class="text-gray-600 text-sm mb-4">
              Sweet mango pudding with fresh fruit topping
            </p>
            <div class="flex justify-between items-center">
              <span
                class="inline-block bg-red-100 text-red-800 text-xs px-2 py-1 rounded-full"
                >Dessert</span
              >
              <!-- <button
                class="text-red-800 hover:text-yellow-600 transition duration-300"
              >
                <i class="fas fa-plus-circle text-xl"></i>
              </button> -->
            </div>
          </div>
        </div>
      </div>

      <div class="text-center mt-12">
        <a
          href="#"
          class="bg-red-800 hover:bg-red-700 text-white px-8 py-3 rounded-full font-medium inline-block transition duration-300"
          >View Full Menu</a
        >
      </div>
    </div>
  </section>

  <!-- Locations Section -->
  <section id="locations" class="py-20 bg-white">
    <div class="container mx-auto px-4">
      <div class="text-center mb-12">
        <h2 class="text-3xl md:text-4xl font-bold mb-2">
          Our <span class="text-red-800">Locations</span>
        </h2>
        <div class="w-24 h-1 bg-yellow-500 mx-auto mb-6"></div>
        <p class="text-gray-600 max-w-2xl mx-auto">
          Visit us at one of our many locations throughout Vietnam
        </p>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
        <!-- Location 1 -->
        <div
          class="bg-white border border-gray-200 rounded-lg p-6 shadow-md hover:shadow-lg transition duration-300"
        >
          <h3 class="text-xl font-bold text-red-800 mb-2">
            Hà Nội - Phạm Ngọc Thạch
          </h3>
          <div class="flex items-start mb-4">
            <i class="fas fa-map-marker-alt text-yellow-600 mt-1 mr-3"></i>
            <p class="text-gray-700">
              P101 - B22 ngõ 97 Phạm Ngọc Thạch, Đống Đa, Hà Nội
            </p>
          </div>
          <div class="flex items-center mb-4">
            <i class="fas fa-phone text-yellow-600 mr-3"></i>
            <p class="text-gray-700">037 9358288</p>
          </div>
          <div class="flex items-center mb-4">
            <i class="fas fa-clock text-yellow-600 mr-3"></i>
            <p class="text-gray-700">9:00 AM - 10:00 PM</p>
          </div>
          <a
            href="#"
            class="text-red-800 hover:text-yellow-600 font-medium flex items-center transition duration-300"
          >
            <span class="mr-2">View on Map</span>
            <i class="fas fa-arrow-right text-sm"></i>
          </a>
        </div>

        <!-- Location 2 -->
        <div
          class="bg-white border border-gray-200 rounded-lg p-6 shadow-md hover:shadow-lg transition duration-300"
        >
          <h3 class="text-xl font-bold text-red-800 mb-2">
            Hà Nội - Nguyễn Văn Lộc
          </h3>
          <div class="flex items-start mb-4">
            <i class="fas fa-map-marker-alt text-yellow-600 mt-1 mr-3"></i>
            <p class="text-gray-700">1 LK6, Nguyễn Văn Lộc, Hà Đông, Hà Nội</p>
          </div>
          <div class="flex items-center mb-4">
            <i class="fas fa-phone text-yellow-600 mr-3"></i>
            <p class="text-gray-700">0856216698</p>
          </div>
          <div class="flex items-center mb-4">
            <i class="fas fa-clock text-yellow-600 mr-3"></i>
            <p class="text-gray-700">9:00 AM - 10:00 PM</p>
          </div>
          <a
            href="#"
            class="text-red-800 hover:text-yellow-600 font-medium flex items-center transition duration-300"
          >
            <span class="mr-2">View on Map</span>
            <i class="fas fa-arrow-right text-sm"></i>
          </a>
        </div>

        <!-- Location 3 -->
        <div
          class="bg-white border border-gray-200 rounded-lg p-6 shadow-md hover:shadow-lg transition duration-300"
        >
          <h3 class="text-xl font-bold text-red-800 mb-2">
            Hà Nội - Ocean Park
          </h3>
          <div class="flex items-start mb-4">
            <i class="fas fa-map-marker-alt text-yellow-600 mt-1 mr-3"></i>
            <p class="text-gray-700">
              Hiệu 1-27 Khu đô thị Vinhomes Ocean Park, Gia Lâm, Hà Nội
            </p>
          </div>
          <div class="flex items-center mb-4">
            <i class="fas fa-phone text-yellow-600 mr-3"></i>
            <p class="text-gray-700">096 169 1629</p>
          </div>
          <div class="flex items-center mb-4">
            <i class="fas fa-clock text-yellow-600 mr-3"></i>
            <p class="text-gray-700">9:00 AM - 10:00 PM</p>
          </div>
          <a
            href="#"
            class="text-red-800 hover:text-yellow-600 font-medium flex items-center transition duration-300"
          >
            <span class="mr-2">View on Map</span>
            <i class="fas fa-arrow-right text-sm"></i>
          </a>
        </div>
      </div>

      <div class="text-center mt-12">
        <a
          href="#"
          class="bg-red-800 hover:bg-red-700 text-white px-8 py-3 rounded-full font-medium inline-block transition duration-300"
          >View All Locations</a
        >
      </div>
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact" class="py-20 bg-gray-100">
    <div class="container mx-auto px-4">
      <div class="text-center mb-12">
        <h2 class="text-3xl md:text-4xl font-bold mb-2">
          Contact <span class="text-red-800">Us</span>
        </h2>
        <div class="w-24 h-1 bg-yellow-500 mx-auto mb-6"></div>
        <p class="text-gray-600 max-w-2xl mx-auto">
          Get in touch with us for reservations, catering inquiries, or feedback
        </p>
      </div>

      <div class="flex flex-col md:flex-row">
        <div class="md:w-1/2 md:pr-8 mb-8 md:mb-0">
          <div class="bg-white rounded-lg shadow-md p-8">
            <h3 class="text-2xl font-bold text-red-800 mb-6">
              Send us a Message
            </h3>
            <form>
              <div class="mb-4">
                <label
                  class="block text-gray-700 text-sm font-medium mb-2"
                  for="name">Full Name</label
                >
                <input
                  class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:border-red-800"
                  type="text"
                  id="name"
                  placeholder="Your name"
                />
              </div>
              <div class="mb-4">
                <label
                  class="block text-gray-700 text-sm font-medium mb-2"
                  for="email">Email Address</label
                >
                <input
                  class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:border-red-800"
                  type="email"
                  id="email"
                  placeholder="Your email"
                />
              </div>
              <div class="mb-4">
                <label
                  class="block text-gray-700 text-sm font-medium mb-2"
                  for="phone">Phone Number</label
                >
                <input
                  class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:border-red-800"
                  type="tel"
                  id="phone"
                  placeholder="Your phone number"
                />
              </div>
              <div class="mb-4">
                <label
                  class="block text-gray-700 text-sm font-medium mb-2"
                  for="message">Message</label
                >
                <textarea
                  class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:border-red-800 h-32"
                  id="message"
                  placeholder="Your message"
                ></textarea>
              </div>
              <button
                type="submit"
                class="bg-red-800 hover:bg-red-700 text-white px-6 py-3 rounded-lg font-medium w-full transition duration-300"
                >Send Message</button
              >
            </form>
          </div>
        </div>

        <div class="md:w-1/2">
          <div class="bg-white rounded-lg shadow-md p-8 mb-8">
            <h3 class="text-2xl font-bold text-red-800 mb-6">
              Contact Information
            </h3>
            <div class="flex items-start mb-6">
              <i class="fas fa-envelope text-yellow-600 mt-1 mr-4 text-xl"></i>
              <div>
                <p class="font-medium text-gray-800">Email Us</p>
                <p class="text-gray-600">info@haochidimsum.vn</p>
              </div>
            </div>
            <div class="flex items-start mb-6">
              <i class="fas fa-phone-alt text-yellow-600 mt-1 mr-4 text-xl"></i>
              <div>
                <p class="font-medium text-gray-800">Call Us</p>
                <p class="text-gray-600">037 9358288</p>
                <p class="text-gray-600">085 6216698</p>
              </div>
            </div>
            <div class="flex items-start">
              <i class="fas fa-clock text-yellow-600 mt-1 mr-4 text-xl"></i>
              <div>
                <p class="font-medium text-gray-800">Opening Hours</p>
                <p class="text-gray-600">
                  Monday to Sunday: 9:00 AM - 10:00 PM
                </p>
              </div>
            </div>
          </div>

          <div class="bg-white rounded-lg shadow-md p-8">
            <h3 class="text-2xl font-bold text-red-800 mb-6">Follow Us</h3>
            <div class="flex space-x-4">
              <!-- <a
                href="#"
                class="bg-red-800 text-white hover:bg-yellow-600 w-10 h-10 rounded-full flex items-center justify-center transition duration-300"
              >
                <i class="fab fa-facebook-f"></i>
              </a>
              <a
                href="#"
                class="bg-red-800 text-white hover:bg-yellow-600 w-10 h-10 rounded-full flex items-center justify-center transition duration-300"
              >
                <i class="fab fa-instagram"></i>
              </a>
              <a
                href="#"
                class="bg-red-800 text-white hover:bg-yellow-600 w-10 h-10 rounded-full flex items-center justify-center transition duration-300"
              >
                <i class="fab fa-twitter"></i>
              </a>
              <a
                href="#"
                class="bg-red-800 text-white hover:bg-yellow-600 w-10 h-10 rounded-full flex items-center justify-center transition duration-300"
              >
                <i class="fab fa-tiktok"></i>
              </a> -->
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="bg-gray-900 text-white pt-12 pb-8">
    <div class="container mx-auto px-4">
      <div class="flex flex-wrap">
        <div class="w-full md:w-1/3 mb-8 md:mb-0">
          <h3 class="text-2xl font-bold mb-4">
            Hao Chi <span class="text-yellow-500">Dimsum</span>
          </h3>
          <p class="text-gray-400 mb-4">
            Authentic Taiwanese dimsum experience with the finest ingredients
            and traditional recipes.
          </p>
          <div class="flex space-x-4">
            <!-- <a
              href="#"
              class="text-gray-400 hover:text-yellow-500 transition duration-300"
            >
              <i class="fab fa-facebook-f"></i>
            </a>
            <a
              href="#"
              class="text-gray-400 hover:text-yellow-500 transition duration-300"
            >
              <i class="fab fa-instagram"></i>
            </a>
            <a
              href="#"
              class="text-gray-400 hover:text-yellow-500 transition duration-300"
            >
              <i class="fab fa-twitter"></i>
            </a>
            <a
              href="#"
              class="text-gray-400 hover:text-yellow-500 transition duration-300"
            >
              <i class="fab fa-tiktok"></i>
            </a> -->
          </div>
        </div>

        <div class="w-full md:w-1/3 mb-8 md:mb-0">
          <h3 class="text-xl font-bold mb-4">Quick Links</h3>
          <ul class="space-y-2">
            <li>
              <a
                href="#home"
                class="text-gray-400 hover:text-yellow-500 transition duration-300"
                >Home</a
              >
            </li>
            <li>
              <a
                href="#about"
                class="text-gray-400 hover:text-yellow-500 transition duration-300"
                >About Us</a
              >
            </li>
            <li>
              <a
                href="#menu"
                class="text-gray-400 hover:text-yellow-500 transition duration-300"
                >Menu</a
              >
            </li>
            <li>
              <a
                href="#locations"
                class="text-gray-400 hover:text-yellow-500 transition duration-300"
                >Locations</a
              >
            </li>
            <li>
              <a
                href="#contact"
                class="text-gray-400 hover:text-yellow-500 transition duration-300"
                >Contact</a
              >
            </li>
          </ul>
        </div>

        <div class="w-full md:w-1/3">
          <h3 class="text-xl font-bold mb-4">Newsletter</h3>
          <p class="text-gray-400 mb-4">
            Subscribe to our newsletter for promotions and updates.
          </p>
          <div class="flex">
            <input
              type="email"
              placeholder="Your email address"
              class="px-4 py-2 rounded-l-lg w-full focus:outline-none"
            />
            <!-- <button
              class="bg-red-800 hover:bg-red-700 text-white px-4 py-2 rounded-r-lg transition duration-300"
            >
              <i class="fas fa-paper-plane"></i>
            </button> -->
          </div>
        </div>
      </div>

      <div
        class="border-t border-gray-800 mt-10 pt-6 flex flex-col md:flex-row justify-between items-center"
      >
        <p class="text-gray-400 text-sm mb-4 md:mb-0">
          © 2025 Hao Chi Dimsum. All rights reserved.
        </p>
        <div class="flex space-x-6">
          <a
            href="#"
            class="text-gray-400 hover:text-yellow-500 text-sm transition duration-300"
            >Privacy Policy</a
          >
          <a
            href="#"
            class="text-gray-400 hover:text-yellow-500 text-sm transition duration-300"
            >Terms of Service</a
          >
        </div>
      </div>
    </div>
  </footer>
</main>

<style>
</style>
