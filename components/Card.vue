<template>
  <div class="p-4">
    <div class="max-w-sm rounded overflow-hidden shadow-lg mb-4 bg-white">
      <div class="h-20 bg-gray-50"></div>
      <div class="px-8 py-4 pb-2 relative">
        <img
          alt="avatar"
          class="w-20 rounded-full absolute -top-10"
          src="~/assets/profile.jpeg"
          width="80px"
        />
        <div class="mb-2 mt-10 flex flex-row">
          <p class="text-lg font-semibold text-current">Angela Jones</p>
          <span
            class="
              inline-flex
              items-center
              justify-center
              px-2
              py-none
              ml-2
              text-xs
              font-bold
              leading-none
              rounded
              bg-yellow-100
              text-yellow-500
            "
            >PRO</span
          >
        </div>
        <div class="mb-2 flex flex-row align-middle">
          <p class="text-xs text-blue-500 font-bold">4.96</p>
          <img src="~/assets/star.svg" alt="star" width="12px" class="ml-2" />
        </div>
        <p class="text-gray-400 text-base w-64 my-6">
          Macroeconomy . Macroeconomy . Statistics . Trading
        </p>
      </div>
      <div class="grid grid-cols-3 px-8 mb-6">
        <div class="text-left text-gray-400">Students</div>
        <div class="text-left text-gray-400">Sessions</div>
        <div class="text-left text-gray-400">Docs</div>
        <div class="text-left text-gray-800 font-bold">852</div>
        <div class="text-left text-gray-800 font-bold">2632</div>
        <div class="text-left text-gray-800 font-bold">46</div>
      </div>
      <div class="px-8 pt-4 pb-12 flex justify-center">
        <button
          type="button"
          class="
            bg-gray-700
            text-white
            py-4
            rounded-xl
            font-medium
            mx-auto
            hover:bg-gray-800
            transition
            duration-200
            each-in-out
            w-96
            shadow-2xl
          "
        >
          Schedule Session
        </button>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
export default {
  props: ['card'],
}
</script>
