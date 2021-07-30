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
            Sign In
          </button>
        </div>
      </form>

      <!-- Start: Direction -->
      <div class="w-full text-center mt-6">
        <span class="font-semibold">Im a new user.</span>
        <span class="ml-1">
          <router-link
            :to="{ name: 'Register', param: {} }"
            class="text-primary font-bold"
            >Sign Up</router-link
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
