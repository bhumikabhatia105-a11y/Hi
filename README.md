# Bunny & Hello Kitty

The site at https://iloveyoudhruv.netlify.app/

One static file — `index.html` — with no build step and no dependencies.
Everything (sky, stars, petals, type, animation) lives in that file.

The only external request is the Cormorant Garamond webfont from Google Fonts.
If it ever fails to load, the page falls back to Iowan Old Style / Palatino /
Georgia and still looks right.

## The page, in order

1. **hero** — "a little something, made just for you" / Bunny
2. the first thing — You make me happy.
3. and then — You do things for me.
4. most of all — You care about me, really care.
5. the truest thing — You've helped me get better, for myself.
6. and one more thing — you are more than enough baby
7. **the promise** — so here's what I need you to know
8. **closing** — I love you, Bunny.

## Deploying

**Drag and drop (easiest)**

1. Go to https://app.netlify.com/projects/iloveyoudhruv/deploys
2. Drag this whole folder onto the deploy drop zone.

Live in a few seconds.

**Or link the repo so it deploys on every push**

In Netlify → project → Build & deploy → link `bhumikabhatia105-a11y/Hi`.
Leave the build command empty and set the publish directory to `.` — there's
nothing to build. After that, every push deploys automatically.

## Editing

**To add another message**, copy one of these blocks and put it wherever you
want it in the sequence:

```html
<section class="reveal">
  <div class="inner">
    <span class="label">the small gold line</span>
    <h2>the big line</h2>
    <p>the message.</p>
  </div>
</section>
```

Keep the `reveal` class or the section never fades in. Everything inside
`.inner` arrives one line after another, in order — that stagger is automatic,
up to six lines.

**Colours** are the variables at the top of the `<style>` block: `--sky-*` for
the gradient, `--glow-warm-*` for the sunrise at the bottom, `--glow-cool` for
the light at the top, and `--gold` / `--coral` / `--cream` for the type.

**Petals and stars** are the `.petal` and `.star` rules plus the two loops in
the `<script>`. Each loop's `count` sets how many there are, with a smaller
number on phones.

## A note on the layering

`body` deliberately has no `background`. The sky is a fixed `<div>`, and a
background on `body` would paint straight over it. If you ever need a
background colour, put it on `html` (as it is now), not `body`.

## Previewing locally

Open `index.html` in a browser. Nothing to install.
