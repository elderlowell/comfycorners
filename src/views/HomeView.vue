<script setup lang="ts">
const goTo = (href: string) => {
  window.open(href, 'blank')
}
</script>

<template>
  <main class="">
    <div class="">
      <section class="relative mb-16 full-width">
        <div
          class="absolute max-w-lg w-[calc(100%-32px)] sm:w-full h-48 bg-emerald-900/60 rounded-xl flex justify-end sm:justify-center items-end font-normal px-8 py-4"
        >
          <div
            class="text-normal sm:text-lg text-white w-full max-w-[150px] sm:max-w-full text-right"
          >
            Welcome to your<br>Home Away From Home
          </div>
        </div>
        <img
          src="@/assets/living-room.jpg"
          alt="Photo of living room furniture by Sherzod Gulomov on Unsplash"
          class="rounded-xl h-48 object-cover w-full"
        />
      </section>
      <section class="text-3xl text-center bg-emerald-900/30 sm:mx-0 px-12 py-16 mb-16">
        <div class="full-width">
          We are a short-term rental hosting company that provides the best comfort possible away
          from home.
        </div>
      </section>
      <section class="mx-auto max-w-sm flex flex-col justify-center items-center gap-4 pb-16">
        <div class="text-md text-xl">Find our properties listed on:</div>
        <button
          @click="goTo('https://airbnb.com')"
          class="bg-[#ff385b] px-6 py-4 text-white rounded-xl text-xl w-48 flex justify-center"
        >
          Airbnb
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="currentColor"
            class="size-6 ml-4"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M13.5 6H5.25A2.25 2.25 0 0 0 3 8.25v10.5A2.25 2.25 0 0 0 5.25 21h10.5A2.25 2.25 0 0 0 18 18.75V10.5m-10.5 6L21 3m0 0h-5.25M21 3v5.25"
            />
          </svg>
        </button>
        <button
          @click="goTo('https://vrbo.com')"
          class="bg-[#1a1e3b] px-6 py-4 text-white rounded-xl text-xl w-48 flex justify-center"
        >
          Vrbo
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="currentColor"
            class="size-6 ml-4"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M13.5 6H5.25A2.25 2.25 0 0 0 3 8.25v10.5A2.25 2.25 0 0 0 5.25 21h10.5A2.25 2.25 0 0 0 18 18.75V10.5m-10.5 6L21 3m0 0h-5.25M21 3v5.25"
            />
          </svg>
        </button>
        <div class="text-xs text-xl max-w-[200px]">
          The following policies are listed on the respectice hosting sites:
          <ul class="mt-2 list-disc list-inside">
            <li>Refund and dispute policy</li>
            <li>Cancelation policy</li>
          </ul>
        </div>
        <div class="text-xs">
          For support inquiries,<br><a href="mailto:support&#64;comfycorners.rentals?subject=Support request from the website" class="text-emerald-800 font-bold underline">please contact us here.</a>
        </div>
      </section>
    </div>
  </main>
</template>
