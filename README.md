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
above the closing `<section class="closing reveal">`:

```html
<section class="reveal">
  <div class="inner">
    <span class="label">the small italic line above</span>
    <h2>the big line</h2>
    <p>the message.</p>
    <p class="always">Always.</p>
  </div>
</section>
```

Each message gets its own full screen, with the warm glow behind it. The
`reveal` class makes it fade up as you scroll to it — don't drop it, or the
message stays invisible. The `label` span and the `always` paragraph are both
optional; leave either out if a message doesn't need it.

**To change the sky**, edit the `--sky-*` variables at the top of the `<style>`
block. `--sky-top` is the dark colour at the top of the screen, `--sky-bot` the
lighter purple at the bottom. The warm glow behind the words is the
`section::before` rule.

**To change the petals or stars**, see the `.petal` and `.star` rules in the
`<style>` block and the two loops in the `<script>` at the bottom. The `count`
variable in each loop controls how many there are (both use a smaller number on
phones).

## Previewing locally

Just open `index.html` in a browser. Nothing else needed.
