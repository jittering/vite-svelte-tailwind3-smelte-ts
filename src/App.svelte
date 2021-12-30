<script lang="ts">
  import { Button, Chip, Card, Image, TextField } from "smelte";

  import "./tailwind-smelte.css";
  import logo from "./assets/svelte.png";
  import Counter from "./lib/Counter.svelte";
</script>

<main>
  <img class="inline" src={logo} alt="Svelte Logo" />
  <h1>Hello Typescript!</h1>

  <Counter />

  <p>
    Visit <a href="https://svelte.dev">svelte.dev</a> to learn how to build Svelte
    apps.
  </p>

  <div class="border-2 m-4 p-4">
    <h2 class="text-zinc-800">Hi Tailwind CSS!</h2>
  </div>

  <h3>And what about Smelte?</h3>

  <div class="flex justify-center gap-4 items-center">
    <TextField label="What is on your mind?" outlined />
    <Button class="">Button</Button>
    <Chip class="" icon="face" removable selectable>test</Chip>
  </div>

  <br />
  <br />

  <Card.Card class="dark:bg-gray-200">
    <div slot="title">
      <Card.Title
        title="The three little kittens"
        subheader="A kitten poem"
        avatar="https://placekitten.com/64/64"
      />
    </div>
    <div slot="media">
      <Image class="w-full" src="https://placekitten.com/300/200" alt="kitty" />
    </div>
    <div slot="text" class="p-5 pb-0 pt-3 text-gray-700 body-2">
      The three little kittens, they lost their mittens,<br />
      And they began to cry,<br />
      "Oh, mother dear, we sadly fear,<br />
      That we have lost our mittens."
    </div>
    <div slot="actions">
      <div class="p-2">
        <Button text>OK</Button>
        <Button text>Meow</Button>
      </div>
    </div>
  </Card.Card>
</main>

<style>
  :root {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
      Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
  }

  main {
    text-align: center;
    padding: 1em;
    margin: 0 auto;
  }

  img {
    height: 16rem;
    width: 16rem;
  }

  h1 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4rem;
    font-weight: 100;
    line-height: 1.1;
    margin: 2rem auto;
    max-width: 14rem;
  }

  p {
    max-width: 14rem;
    margin: 1rem auto;
    line-height: 1.35;
  }

  @media (min-width: 480px) {
    h1 {
      max-width: none;
    }

    p {
      max-width: none;
    }
  }
</style>
