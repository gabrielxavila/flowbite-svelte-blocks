<script lang="ts">
  import { Section, Register } from '$lib';
  import { ExampleDiv, SectionHeader, SectionBlock, MetaTag } from '../utils';
  import { Button, Checkbox, Label, Input } from 'flowbite-svelte';
  const breadcrumb_title = 'Reset Password Forms';
  const title = 'Reset password';
  const dir = 'marketing';
  const description =
    'Use a collection of reset password forms based on multiple layouts to let your users change their password after going through the account recovery email.';
</script>

<MetaTag {breadcrumb_title} {title} {dir} {description} />

<SectionHeader
  category="marketing"
  title="Svelte {breadcrumb_title} - Flowbite"
  {breadcrumb_title}
  {description}
/>

<SectionBlock title="Default reset password page">
  Use this example with an email input and two password input fields to let the user change their
  password after receiving the account recovery email.
</SectionBlock>

<ExampleDiv>
  <Section name="reset">
    <Register href="/">
      <svelte:fragment slot="top">
        <img class="w-8 h-8 mr-2" src="/images/logo.svg" alt="logo" />
        Flowbite
      </svelte:fragment>
      <div class="p-6 space-y-4 md:space-y-6 sm:p-8">
        <form class="flex flex-col space-y-6" action="/">
          <h3 class="text-xl font-medium text-gray-900 dark:text-white p-0">Change Password</h3>
          <Label class="space-y-2">
            <span>Your email</span>
            <Input type="email" name="email" placeholder="name@company.com" required />
          </Label>
          <Label class="space-y-2">
            <span>Your password</span>
            <Input type="password" name="password" placeholder="•••••" required />
          </Label>
          <Label class="space-y-2">
            <span>Confirm password</span>
            <Input type="password" name="confirm-password" placeholder="•••••" required />
          </Label>
          <div class="flex items-start">
            <Checkbox
              >I accept the <a
                class="font-medium text-primary-600 hover:underline dark:text-primary-500"
                href="/"
              >
                Terms and Conditions</a
              ></Checkbox
            >
          </div>
          <Button type="submit" class="w-full1">Reset passwod</Button>
        </form>
      </div>
    </Register>
  </Section>
</ExampleDiv>
