# Account Recovery Form

[Demo](https://flowbite-svelte-blocks.vercel.app/marketing/account-recovery)

## Example usage

```html
<script lang="ts">
  import { ForgotPassword, ForgotPasswordHeader } from 'flowbite-svelte-blocks';
</script>

<ForgotPasswordHeader src="/images/logo.svg" alt="logo" href="/"> Flowbite </ForgotPasswordHeader>
<ForgotPassword>
  <h1
    class="mb-1 text-xl font-bold leading-tight tracking-tight text-gray-900 md:text-2xl dark:text-white"
  >
    Forgot your password?
  </h1>
  <p class="font-light text-gray-500 dark:text-gray-400">
    Don't fret! Just type in your email and we will send you a code to reset your password!
  </p>
  <form class="mt-4 space-y-4 lg:mt-5 md:space-y-5">
    <div>
      <label for="email" class="block mb-2 text-sm font-medium text-gray-900 dark:text-white"
        >Your email</label
      >
      <input type="email" name="email" id="email" placeholder="name@company.com" required />
    </div>
    <div class="flex items-start">
      <div class="flex items-center h-5">
        <Checkbox id="terms" aria-describedby="terms" required
          >I accept the
          <a class="font-medium text-primary-600 hover:underline dark:text-primary-500" href="/"
            >Terms and Conditions</a
          ></Checkbox
        >
      </div>
    </div>
    <button type="submit" color="red">Reset password</button>
  </form>
</ForgotPassword>
```
