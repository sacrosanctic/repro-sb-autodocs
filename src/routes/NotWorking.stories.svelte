<script context="module" lang="ts">
  import type { Meta } from "@storybook/svelte";

  import MyComponent from "./Counter.svelte";

  export const meta: Meta = {
    component: MyComponent,
    tags: ["autodocs"],
    argTypes: {},
  };
</script>

<script lang="ts">
  import { Story, Template } from "@storybook/addon-svelte-csf";
</script>

<Template let:args>
  <MyComponent {...args} />
</Template>

<Story name="base" />
