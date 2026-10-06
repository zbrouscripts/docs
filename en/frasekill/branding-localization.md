# Branding and languages

## Logo

Replace:

```text
web/logo.png
```

Keep the same filename. The logo is excluded from escrow so server owners can replace it easily.

## Menu colours

The three global menu colours are independent:

```lua
Config.UI.AccentColor = '#0e58d8'
Config.UI.BackgroundColor = '#15181e'
Config.UI.BaseColor = '#1a1e25'
```

They are also available as colour pickers in Script settings. Classic remains a solid surface. Liquid Glass stays optional and is **not** enabled by changing colours.

## Languages

English is the default. The built-in selector includes:

- English
- Español
- Português
- Français
- Türkçe
- Deutsch
- Italiano
- Polski

Player language preference is saved. Admin and normal player UI use the same localization system.
