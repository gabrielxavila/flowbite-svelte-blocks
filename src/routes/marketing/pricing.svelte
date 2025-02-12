<script lang="ts">
  import {
    Section,
    PricingBodyHead,
    PricingCard,
    PricingItemWrapper,
    PricingHead,
    PricingItem
  } from '$lib';
  import { ExampleDiv, SectionHeader, SectionBlock, MetaTag } from '../utils';
  import { Button } from 'flowbite-svelte';
  const breadcrumb_title = 'Pricing Tables';
  const title = 'Pricing';
  const dir = 'marketing';
  const description =
    'Get started with a collection of responsive pricing sections to show the pricing plan to your potential customers based on multiple sizes, styles, and layouts.';
</script>

<MetaTag {breadcrumb_title} {title} {dir} {description} />

<SectionHeader
  category="marketing"
  title="Svelte {breadcrumb_title} - Flowbite"
  {breadcrumb_title}
  {description}
/>

<SectionBlock title="Default pricing table">
  Use this example of three pricing cards showcasing the pricing plan title, description, feature
  list, and CTA button.
</SectionBlock>

<ExampleDiv>
  <Section name="pricing">
    <PricingHead>
      <svelte:fragment slot="h2">Designed for business teams like yours</svelte:fragment>
      <svelte:fragment slot="paragraph"
        >Here at Flowbite we focus on markets where technology, innovation, and capital can unlock
        long-term value and drive economic growth.</svelte:fragment
      >
    </PricingHead>
    <div class="space-y-8 lg:grid lg:grid-cols-3 sm:gap-6 xl:gap-10 lg:space-y-0">
      <PricingCard>
        <PricingBodyHead>
          <svelte:fragment slot="h3">Starter</svelte:fragment>
          <svelte:fragment slot="paragraph">
            Best option for personal use & for your next project.
          </svelte:fragment>
          <svelte:fragment slot="price">
            <span class="mr-2 text-5xl font-extrabold">$29</span>
            <span class="text-gray-500 dark:text-gray-400">/month</span>
          </svelte:fragment>
        </PricingBodyHead>
        <PricingItemWrapper>
          <PricingItem>
            <span>Individual configuration</span>
          </PricingItem>
          <PricingItem>
            <span>No setup, or hidden fees</span>
          </PricingItem>
          <PricingItem>
            <span>Team size: <span class="font-semibold">1 developer</span></span>
          </PricingItem>
          <PricingItem>
            <span>Premium support: <span class="font-semibold">6 months</span></span>
          </PricingItem>
          <PricingItem>
            <span>Free updates: <span class="font-semibold">6 months</span></span>
          </PricingItem>

          <svelte:fragment slot="btn">
            <Button color="red">Get started</Button>
          </svelte:fragment>
        </PricingItemWrapper>
      </PricingCard>

      <PricingCard>
        <PricingBodyHead>
          <svelte:fragment slot="h3">Company</svelte:fragment>
          <svelte:fragment slot="paragraph">
            Relevant for multiple users, extended & premium support.
          </svelte:fragment>
          <svelte:fragment slot="price">
            <span class="mr-2 text-5xl font-extrabold">$99</span>
            <span class="text-gray-500 dark:text-gray-400" dark:text-gray-400>/month</span>
          </svelte:fragment>
        </PricingBodyHead>
        <PricingItemWrapper>
          <PricingItem>
            <span>Individual configuration</span>
          </PricingItem>
          <PricingItem>
            <span>No setup, or hidden fees</span>
          </PricingItem>
          <PricingItem>
            <span>Team size: <span class="font-semibold">10 developer</span></span>
          </PricingItem>
          <PricingItem>
            <span>Premium support: <span class="font-semibold">24 months</span></span>
          </PricingItem>
          <PricingItem>
            <span>Free updates: <span class="font-semibold">24 months</span></span>
          </PricingItem>

          <svelte:fragment slot="btn">
            <Button color="red">Get started</Button>
          </svelte:fragment>
        </PricingItemWrapper>
      </PricingCard>

      <PricingCard>
        <PricingBodyHead>
          <svelte:fragment slot="h3">Enterprise</svelte:fragment>
          <svelte:fragment slot="paragraph">
            Best for large scale uses and extended redistribution rights.
          </svelte:fragment>
          <svelte:fragment slot="price">
            <span class="mr-2 text-5xl font-extrabold">$499</span>
            <span class="text-gray-500 dark:text-gray-400">/month</span>
          </svelte:fragment>
        </PricingBodyHead>
        <PricingItemWrapper>
          <PricingItem>
            <span>Individual configuration</span>
          </PricingItem>
          <PricingItem>
            <span>No setup, or hidden fees</span>
          </PricingItem>
          <PricingItem>
            <span>Team size: <span class="font-semibold">100+ developer</span></span>
          </PricingItem>
          <PricingItem>
            <span>Premium support: <span class="font-semibold">36 months</span></span>
          </PricingItem>
          <PricingItem>
            <span>Free updates: <span class="font-semibold">36 months</span></span>
          </PricingItem>

          <svelte:fragment slot="btn">
            <Button color="red">Get started</Button>
          </svelte:fragment>
        </PricingItemWrapper>
      </PricingCard>
    </div>
  </Section>
</ExampleDiv>
