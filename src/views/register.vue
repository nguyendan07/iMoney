<template>
  <div class="mt-8">
    <div class="container mx-auto px-8">
      <!-- Start: From -->
      <form
        @submit.prevent="onSubmit"
        method="post"
        class="flex flex-col justify-start space-y-6"
      >
        <div class="row">
          <label class="flex flex-col" for="fullName">
            <span class="font-semibold">Full Name</span>
            <input
              id="fullName"
              class="px-4 py-3 rounded-lg mt-1 border border-gray-100"
              type="text"
              placeholder="Full Name"
            />
          </label>
        </div>
        <div class="row">
          <label class="flex flex-col" for="email">
            <span class="font-semibold">Email Address</span>
            <input
              id="email"
              class="px-4 py-3 rounded-lg mt-1 border border-gray-100"
              type="email"
              placeholder="example@mail.com"
              autocomplete="username"
            />
          </label>
        </div>
        <div class="row">
          <label class="flex flex-col" for="password">
            <span class="font-semibold">Password</span>
            <input
              id="password"
              class="px-4 py-3 rounded-lg mt-1 border border-gray-100"
              type="password"
              placeholder=""
              autocomplete="current-password"
            />
          </label>
        </div>
        <div class="row">
          <button
            type="submit"
            class="
              py-3
              text-center
              w-full
              bg-primary
              text-white
              font-bold
              rounded-lg
            "
          >
            Sign Up
          </button>
        </div>
      </form>

      <!-- Start: Direction -->
      <div class="w-full text-center mt-6">
        <span class="font-semibold">Im alreadly a member.</span>
        <span class="ml-1">
          <router-link
            :to="{ name: 'Login', param: {} }"
            class="text-primary font-bold"
            >Sign In</router-link
          >
        </span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  setup() {
    function onSubmit() {}
    return { onSubmit };
  },
};
</script>
