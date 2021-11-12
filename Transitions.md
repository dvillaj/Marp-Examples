---
title: Marp CLI experimental transitions
_class: lead gaia
theme: gaia
style: |
  pre {
    font-size: 60px;
  }
marp: true
---

### Marp CLI experimental

# Transitions 🪄

---

![bg opacity](https://images.unsplash.com/photo-1627597606331-df0d125f37b8?crop=entropy&cs=tinysrgb&fit=crop&fm=jpg&h=720&ixid=MnwxfDB8MXxyYW5kb218MHx8fHx8fHx8MTYzMDA4OTM1Nw&ixlib=rb-1.2.1&q=80&w=1280)

<!-- _transition: fade -->
<!-- _class: invert -->

## Fade transition

```yaml
transition: fade
```

---

![bg opacity](https://images.unsplash.com/photo-1629673460055-b3a6cf1df9d8?crop=entropy&cs=tinysrgb&fit=crop&fm=jpg&h=720&ixid=MnwxfDB8MXxyYW5kb218MHx8fHx8fHx8MTYzMDA4OTU0NA&ixlib=rb-1.2.1&q=80&w=1280)

<!-- _transition: cover -->

## Cover transition

```yaml
transition: cover
```

---

![bg](https://images.unsplash.com/photo-1628763228722-b11a9c545ed7?crop=entropy&cs=tinysrgb&fit=crop&fm=jpg&h=720&ixid=MnwxfDB8MXxyYW5kb218MHx8fHx8fHx8MTYzMDA4OTU4Mg&ixlib=rb-1.2.1&q=80&w=1280)

<!-- _transition: reveal -->
<!-- _class: invert -->

## Reveal transition

```yaml
transition: reveal
```

---

![bg](https://images.unsplash.com/photo-1629194888885-415f67fc9bc7?crop=entropy&cs=tinysrgb&fit=crop&fm=jpg&h=720&ixid=MnwxfDB8MXxyYW5kb218MHx8fHx8fHx8MTYzMDA4OTYyNA&ixlib=rb-1.2.1&q=80&w=1280)

<!-- _transition: implode -->

## Implode transition

```yaml
transition: implode
```

---

![bg](https://images.unsplash.com/photo-1627691541764-85b6e9003bec?crop=entropy&cs=tinysrgb&fit=crop&fm=jpg&h=720&ixid=MnwxfDB8MXxyYW5kb218MHx8fHx8fHx8MTYzMDA4OTY1OQ&ixlib=rb-1.2.1&q=80&w=1280)

<!-- _transition: explode -->
<!-- _class: invert -->

## Explode transition

```yaml
transition: explode
```

---

<!-- _class: lead -->

It's going to become an experimental option of Marp CLI.

```sh
marp --template bespoke --bespoke.transition ./transition.md
```

Transitions are using **[Shared Element Transition API](https://github.com/WICG/shared-element-transitions)** proposal, and working only in Marp CLI preview mode `--preview` and supported browsers like Chromium with enabled `documentTransition API` from `about://flags` or Origin Trials.
