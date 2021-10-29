<image src=".github/OMGEX.png" width="50" align="left">

# OMGEX ("OMG Extended")

Extended profile features for OMG.LOL, your favorite pigeon community.

OMGEX supports all default OMG.LOL themes. Issues and pull requests are welcome, so fire away!

## Installation

Add the following to your OMG.LOL page `<head>`:

```js
<script src="https://cdn.jsdelivr.net/gh/litdevs/omgex@latest/OMGEX.js"></script>
<script>
window.addEventListener('load', function() {
    OMGEX({zodiac: "♓", birthday: "March 5", timezone: "CET", terminalKonami: true});
});
</script>
```

## Configuration

OMGEX has a few settings you can use to customize what it displays. You'll need at least one, or else it'll throw an error.

### A new option isn't working properly!

This may either be caching issues, or because the feature is broken. You can try going [here](https://purge.jsdelivr.net/gh/litdevs/omgex@latest/OMGEX.js) to clear the jsDelivr cache - if it says it's throttled, wait until the `throttlingReset` (in seconds) has passed and try clearing the jsDelivr cache again.

If it does not say it's throttled, go to your OMG.LOL page and see if it works now - note that you may have to clear your own cache as well. If it's still broken, [submit a bug report](https://github.com/LITdevs/OMGEX/issues/new). If you have a fix, pull requests are welcome.

### zodiac

This displays your zodiac sign next to your pronouns.

### birthday

This displays your birthday next to your occupation and location.

### timezone

This displays your current time next to your occupation and location. Note that this is experimental, and output may vary across browsers and machines.

### terminalKonami

Setting this to `true` will redirect the user to [terminal.land](https://terminal.land/) when the Konami code is entered.

### fixIcons

Using the `/fa-icon/` format in a OMG.LOL profile item assumes you always want to use `fa-solid.` fixIcons is enabled by default, and will allow you to do (for example) `/fa-brands fa-amazon/` without problems. If it is causing problems for you, just set it to `false`.

This was added due to https://github.com/neatnik/omg.lol/issues/112.

### promoteOMGEX

OMGEX adds a link to its GitHub repo in the footer, but this can be disabled if you prefer - just set this option to `false`. You won't really have to do this if you're already hiding the footer, since it won't display.
