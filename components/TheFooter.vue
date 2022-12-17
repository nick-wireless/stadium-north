<template>
  <footer class="bg-gray-800" aria-labelledby="footer-heading">
    <h2 id="footer-heading" class="sr-only">Footer</h2>
    <section>
      <div class=" bg-teal-200 mt-8 lg:mt-16 py-6 ">
        <achnowledge-country />
      </div>
    </section>
    <div class="mx-auto max-w-7xl py-12 px-4 sm:px-6 lg:py-16 lg:px-8">
      <div class="xl:grid xl:grid-cols-3 xl:gap-8">
        <div class="grid grid-cols-2 gap-8 xl:col-span-2">
          <div class="md:grid md:grid-cols-2 md:gap-8">
            <div>
              <h3 class="text-base font-medium text-white">About</h3>
              <ul role="list" class="mt-4 space-y-4">
                <li v-for="item in navigation.about" :key="item.name">
                  <a :href="item.href" class="text-base text-gray-300 hover:text-white">{{ item.name }}</a>
                </li>
              </ul>
            </div>
            <div class="mt-12 md:mt-0">
              <h3 class="text-base font-medium text-white">Support</h3>
              <ul role="list" class="mt-4 space-y-4">
                <li v-for="item in navigation.support" :key="item.name">
                  <a :href="item.href" class="text-base text-gray-300 hover:text-white">{{ item.name }}</a>
                </li>
              </ul>
            </div>
          </div>
          <div class="md:grid md:grid-cols-2 md:gap-8">
            <div>
              <h3 class="text-base font-medium text-white">Process</h3>
              <ul role="list" class="mt-4 space-y-4">
                <li v-for="item in navigation.process" :key="item.name">
                  <a :href="item.href" class="text-base text-gray-300 hover:text-white">{{ item.name }}</a>
                </li>
              </ul>
            </div>
            <div class="mt-12 md:mt-0">
              <h3 class="text-base font-medium text-white">Platform</h3>
              <ul role="list" class="mt-4 space-y-4">
                <li v-for="item in navigation.platform" :key="item.name">
                  <a :href="item.href" class="text-base text-gray-300 hover:text-white">{{ item.name }}</a>
                </li>
              </ul>
            </div>
          </div>
        </div>
        <div class="mt-8 xl:mt-0">
          <h3 class="text-base font-medium text-white">Subscribe to our newsletter</h3>
          <p class="mt-4 text-base text-gray-300">The latest news, announcements and tickets, sent to your inbox periodically.
          </p>
          <form class="mt-4 sm:flex sm:max-w-md">
            <label for="email-address" class="sr-only">Email address</label>
            <input type="email" name="email-address" id="email-address" autocomplete="email" required=""
              class="w-full min-w-0 appearance-none rounded-md border border-transparent bg-white py-2 px-4 text-base text-gray-900 placeholder-gray-500 focus:border-white focus:placeholder-gray-400 focus:outline-none focus:ring-2 focus:ring-white focus:ring-offset-2 focus:ring-offset-gray-800"
              placeholder="Enter your email" />
            <div class="mt-3 rounded-md sm:mt-0 sm:ml-3 sm:flex-shrink-0">
              <button type="submit"
                class="flex w-full items-center justify-center rounded-md border border-transparent bg-indigo-500 py-2 px-4 text-base font-medium text-white hover:bg-indigo-600 focus:outline-none focus:ring-2 focus:ring-indigo-500 focus:ring-offset-2 focus:ring-offset-gray-800">Subscribe</button>
            </div>
          </form>
        </div>
      </div>
      <div class="mt-8 border-t border-gray-700 pt-8 md:flex md:items-center md:justify-between">
        <div class="flex space-x-6 md:order-2">
          <a v-for="item in navigation.social" :key="item.name" :href="item.href"
          class="text-gray-400 hover:text-gray-300">
          <span class="sr-only">{{ item.name }}</span>
          <component :is="item.icon" class="h-6 w-6" aria-hidden="true" />
        </a>
      </div>
      <p class="pt-8 text-base text-gray-400 md:order-1 md:mt-0 mr-4 ">TLDR & Summary: Australia's Darwin city's plan for a world class stadium.</p>
      <p class="pt-8 text-base text-gray-400 md:order-1 md:mt-0">&copy; 2023 Stadiums North Australia. All rights reserved.</p>
      </div>
    </div>
  </footer>
</template>

<script setup>
import { defineComponent, h } from 'vue'

const navigation = {
  about: [
    { name: 'About', href: '#' },
    { name: 'Partners', href: '#' },
    { name: 'Careers', href: '#' },
    { name: 'Press', href: '#' },
  ],
  support: [
    { name: 'Announcements', href: '#' },
    { name: 'Membership', href: '#' },
    { name: 'Polls', href: '#' },
    { name: 'Steering Committees', href: '#' },
    { name: 'Newsletter', href: '#' },
    { name: 'Community', href: '#' },
  ],
  process: [
    { name: 'Sports 2050 Plan', href: '#' },
    { name: 'Site Selection', href: '#' },
    { name: 'Designs', href: '#' },
    { name: 'Partners', href: '#' },
    { name: 'Development', href: '#' },
  ],
  platform: [
    { name: 'Licences', href: '#' },
    { name: 'Terms & Condition', href: '#' },
    { name: 'Legal', href: '#' },
  ],
}

</script>