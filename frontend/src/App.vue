<template>
  <div>
    <header class="relative z-50 w-full h-24">
      <div class="container flex items-center justify-center h-full max-w-6xl px-8 mx-auto sm:justify-between xl:px-0">
        <a href="/" class="relative flex items-center inline-block h-5 h-full font-black leading-none">
          <svg class="w-auto h-6 text-indigo-600 fill-current" viewBox="0 0 194 116" xmlns="http://www.w3.org/2000/svg">
            <g fill-rule="evenodd">
              <path d="M96.869 0L30 116h104l-9.88-17.134H59.64l47.109-81.736zM0 116h19.831L77 17.135 67.088 0z" />
              <path d="M87 68.732l9.926 17.143 29.893-51.59L174.15 116H194L126.817 0z" />
            </g>
          </svg>
          <span class="ml-3 text-xl text-gray-800">Student Helper<span class="text-pink-500">.</span></span>
        </a>

        <nav
          id="nav"
          class="absolute top-0 left-0 z-50 flex flex-col items-center justify-between hidden w-full h-64 pt-5 mt-24 text-sm text-gray-800 bg-white border-t border-gray-200 md:w-auto md:flex-row md:h-24 lg:text-base md:bg-transparent md:mt-0 md:border-none md:py-0 md:flex md:relative"
        >
          <router-link :to="{ name: 'home' }" class="ml-0 mr-0 font-bold duration-100 md:ml-8 md:mr-3 transition-color hover:text-indigo-600">Utama</router-link>
          <router-link :to="{ name: 'donasi' }" class="ml-0 mr-0 font-bold duration-100 md:mr-3 lg:mr-8 transition-color hover:text-indigo-600 pl-4">Donasi</router-link>
          <router-link :to="{ name: 'kerja' }" class="ml-0 mr-0 font-bold duration-100 md:mr-3 lg:mr-8 transition-color hover:text-indigo-600">Lowongan</router-link>
        </nav>

        <div
          class="absolute left-0 flex-col items-center justify-center hidden w-full pb-8 mt-48 border-b border-gray-200 md:relative md:w-auto md:bg-transparent md:border-none md:mt-0 md:flex-row md:p-0 md:items-end md:flex md:justify-between"
        >
          <router-link :to="{ name: 'login' }" class="relative z-40 px-3 py-2 mr-0 text-sm font-bold bg bg-pink-500 rounded-lg text-white md:px-5 sm:mr-3 md:mt-0">Masuk</router-link>
          <router-link
            :to="{ name: 'signup' }"
            class="relative z-40 inline-block w-auto h-full px-5 py-3 text-sm font-bold leading-none transition-all transition duration-100 duration-300 bg bg-indigo-500 rounded-lg text-white rounded shadow-md fold-bold sm:w-full lg:shadow-none hover:shadow-xl"
            >Daftar</router-link
          >
        </div>

        <div id="nav-mobile-btn" class="absolute top-0 right-0 z-50 block w-6 mt-8 mr-10 cursor-pointer select-none md:hidden sm:mt-10">
          <span class="block w-full h-1 mt-2 duration-200 transform bg-gray-800 rounded-full sm:mt-1"></span>
          <span class="block w-full h-1 mt-1 duration-200 transform bg-gray-800 rounded-full"></span>
        </div>
      </div>
    </header>
    <!--- render router view -->
    <router-view></router-view>
  </div>
</template>
