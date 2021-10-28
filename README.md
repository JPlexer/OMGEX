# OMGEX

Extended profile features for OMG.LOL

## Installation

Add the following to your OMG.LOL page `<head>`:

```js
<script src="https://cdn.jsdelivr.net/gh/litdevs/omgex/OMGEX.js"></script>
<script>
window.addEventListener('load', function() {
    OMGEX({zodiac: "♓", birthday: "March 5"});
});
</script>
```

## Configuration

OMGEX has a few settings you can use to customize what it displays. You'll need at least one, or else it'll throw an error.

### zodiac

This displays your zodiac sign next to your pronouns.

### birthday

This displays your birthday next to your occupation and location.

### terminalKonami

Setting this to `true` will redirect the user to [terminal.land](https://terminal.land/) when the Konami code is entered.

### promoteOMGEX

OMGEX adds a link to its GitHub repo in the footer, but this can be disabled if you prefer - just set this option to `false`. You won't really have to do this if you're already hiding the footer, since it won't display.
