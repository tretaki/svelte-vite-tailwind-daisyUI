<script>
  import logo from "./assets/svelte.png";
  import Counter from "./components/Counter.svelte";
  import Article from "./components/Article.svelte";
  import Card from "./components/Card.svelte";

  const cardData = {
    cardTitle: "Happy Svelting",
    cardText:
      "Svelte is a radical new approach to building user interfaces. Whereas traditional frameworks like React and Vue do the bulk of their work in the browser, Svelte shifts that work into a compile step that happens when you build your app.",
  };
</script>

<div class="container mx-auto px-4">
  <Article>
    <h1>Svelte with Tailwind CSS and daisyUI</h1>
    <h2>Let's see how this works</h2>
    <p>
      Here is the some text using the tailwind typograpy plugin. Lorem ipsum
      dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
      incididunt ut labore et dolore magna aliqua. Orci a scelerisque purus
      semper eget duis at. Laoreet non curabitur gravida arcu ac tortor
      dignissim. Faucibus in ornare quam viverra orci.
    </p>
    <blockquote>
      <p>
        Only two things are infinite, the universe and human stupidity, and I'm
        not sure about the former. <br />
      </p>
    </blockquote>
    <em class="text-sm">- Albert Einstein</em>

    <p>Loading button example:</p>
    <div class="flex justify-center m-10">
      <button class="btn btn-primary loading lowercase">Loading ...</button>
    </div>

    <p>Counter example:</p>
    <Counter />
  </Article>

  <div class="flex justify-center m-10">
    <p>Grid example:</p>
  </div>
  <div class="flex justify-center m-10">
    <div class="grid grid-cols-3 gap-6">
      <Card {...cardData}><img src={logo} alt="svelte logo" width="200" /></Card
      >
      <Card {...cardData}><img src={logo} alt="svelte logo" width="200" /></Card
      >
      <Card {...cardData}><img src={logo} alt="svelte logo" width="200" /></Card
      >
    </div>
  </div>
  <div class="flex justify-center m-10">
    Toggle button example:
    <input type="checkbox" class="toggle toggle-primary mx-2" checked />
  </div>

  <div class="flex justify-center m-10">
    <p>Code mockup example:</p>
  </div>
  <div class="flex justify-center m-10">
    <div class="mockup-code">
      <pre data-prefix="$"><code>npm i daisyui</code></pre>
      <pre data-prefix=">" class="text-warning"><code>installing...</code></pre>
      <pre data-prefix=">" class="text-success"><code>Done!</code></pre>
    </div>
  </div>
</div>
