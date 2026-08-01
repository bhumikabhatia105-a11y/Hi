# iloveyoudhruv

The site at https://iloveyoudhruv.netlify.app/

It's a single static file — `index.html` — with no build step, no dependencies,
and nothing to install. Everything (styles, petals, animations) is inside that
one file.

## Deploying

**Drag and drop (easiest)**

1. Go to https://app.netlify.com/projects/iloveyoudhruv/deploys
2. Drag this whole folder onto the deploy drop zone.

That's it — it goes live in a few seconds.

**Or link the repo so it deploys on every push**

In Netlify → project → Build & deploy → link `bhumikabhatia105-a11y/Hi`.
Leave the build command empty and set the publish directory to `.` (the repo
root), since there's nothing to build. After that, every push to the branch
you pick deploys automatically.

## Editing

**To add another message**, copy one of these blocks in `index.html` and put it
above the closing `<footer class="closing">`:

```html
<section class="message reveal">
  <h2>the heading</h2>
  <p>the message.</p>
  <p class="always">Always.</p>
</section>
```

The `reveal` class is what makes it fade in as you scroll to it. The
`class="always"` paragraph is the italic pink sign-off — leave it out if a
message doesn't need one.

**To change the colours**, edit the variables at the top of the `<style>` block
(`--bg-top`, `--accent`, and so on).

**To change the petals**, see the `.petal` rules in the `<style>` block and the
petal loop in the `<script>` at the bottom. `count` controls how many fall.

## Previewing locally

Just open `index.html` in a browser. Nothing else needed.
