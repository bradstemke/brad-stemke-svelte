# bradstemke.com

Rebuilding my personal website using Svelte, and documenting it here.

## Initial Thoughts

As I begin to learn about Svelte, I took an approach that I often do when looking into new technology. I love podcasts and find them to be a fantastic way to learn about new things, especially code related topics. I listened to a couple podcast episodes from developers I follow and trust to hear their takes. Both episodes were really informative and gave me a good high level mindset to use while I started on this build.
- https://syntax.fm/show/413/how-to-do-things-in-svelte
- https://syntax.fm/show/390/from-react-to-sveltekit

I also plan on completing the tutorial that Svelte offers on their website.

As I have started refactoring and rebuilding my personal website using Svelte, I have noticed a few high level things

1. Svelte just works. From installation to creating components, everything has been very natural-feeling, practical in approach, and simple. For example, placing components into the /lib folder and being able to call them in the project so simply is amazing. 

2. While I have only created a single component, as I continue with the rest, I am already a huge fan of the scoped styling and overall approach taken in regards to styling. Writing plain CSS again feels like coming home. Not needing to be concerned with a CSS-in-JS approach or methods feels refreshing.

3. Coding and frameworks can, at times, be as complex as you allow them to be. At every turn, I can tell that the community and team behind Svelte have taken the developer experience as a top priority, and that becomes increasingly apparent the more I work with it.

4. The way it handles reactivity feels like pure magic. I am mostly building static components for now, but I did read into this and am going to find a way to incorporate and learn more about it on this rebuild.

5. When I finish websites or software work, I really enjoy running speed tests and measuring that what has been built is running as efficiently as possible. I have a strong feeling that the speed tests from this build will outperform the ones for the same site built in React. I can also tell that the bundle size will be much smaller.

6. Given Svelte's direct DOM manipulation, I am excited to see how animations are handled in the browser. I imagine they will be a little smoother.

7. A few things I haven't needed yet but want to read more on are stores and motion.

8. As I add more components, a Google Font, and look at how it handles images, I appreciate Svelte's overall encouragement and approach to not overthink or overcomplicate things. I am really excited to complete this build, and it seems likely that it will actually become my main build for use on my domain, replacing the React one!

Just a few thoughts I wanted to document as I continue with this project!

## Creating a project

If you're seeing this, you've probably already done this step. Congrats!

```bash
# create a new project in the current directory
npm create svelte@latest

# create a new project in my-app
npm create svelte@latest my-app
```

## Developing

Once you've created a project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```bash
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

## Building

To create a production version of your app:

```bash
npm run build
```

You can preview the production build with `npm run preview`.

> To deploy your app, you may need to install an [adapter](https://kit.svelte.dev/docs/adapters) for your target environment.
