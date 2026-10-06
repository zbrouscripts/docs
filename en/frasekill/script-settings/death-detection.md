# Death detection

This section decides **when and where FraseKill may appear**.

On most servers you can leave the medical adapter on **Auto**. You can also choose whether FraseKill appears at incapacitated/last-stand or final death.

## Kill zones

Zones never grant FraseKill access. The killer still needs their normal player access.

Create circular zones with a centre and radius directly from Script settings:

- **Outside allowed + Block zone** — FraseKill works normally except inside those zones.
- **Outside blocked + Allow zone** — FraseKill works only inside the allowed zones.

If Allow and Block zones overlap, **Block wins**.

**Use my position** captures the administrator's current position. **Preview radius** temporarily hides the panel and draws the radius in the world: blue for Allow and red for Block.

The real decision is server-side using the victim's death position. Being inside a zone never replaces player access.

See **Medical compatibility** for the supported list.
