# Wine themes

Windows applications that you can run via Wine often look like Windows 95,
especially in Wine 6 and below, which shipped no default themes.
Here you can find some color themes which should make them look somewhat
nicer without having to tune everything manually or resorting to full-fledged
themes.

To apply a theme, run `wine regedit "THEMEFILE.reg"`. You may have to restart
Windows applications that you have running afterwards in order for the changes
to take effect.

The themes are provided as `.reg` files, and not `.theme`, because, it seems,
the latter format only allows [a subset of color entries to be specified][1],
and Wine ignores other definitions.

Note that at least as late as Wine 6, some color entries are ignored entirely,
and other ones are used instead. For example, `MenuHilight` color seems unused,
as `Hilight` is used instead.

[1]: https://learn.microsoft.com/en-us/windows/win32/controls/themesfileformat-overview#control-panelcolors-section
